# Corypheus Red Lyrium Brutal

This repository contains a practical texture-generation starter for a Dragon Age 2 Corypheus-inspired red lyrium armor skin.

Important note:
- This environment cannot generate a valid game-ready ERF package or a final binary asset with the exact original game asset path without the original DA2 files and mod toolchain.
- What is included here is a generator script that creates high-resolution texture maps locally and a packaging guide for DA2 modding.
- The final game-ready files should be exported to DDS and then inserted into the corresponding armor asset, or packed into ERF by your DA2 mod tool.

Included:
- `generate_red_lyrium.py` — produces a dark metal albedo texture and companion maps.
- `requirements.txt` — Python dependencies.
- `README.md` — instructions.

Generation script outputs:
- `output/CorypheusRedLyrium_Brutal_Albedo.png`
- `output/CorypheusRedLyrium_Brutal_Albedo.dds`
- `output/CorypheusRedLyrium_Brutal_Normal.png`
- `output/CorypheusRedLyrium_Brutal_Normal.dds`
- `output/CorypheusRedLyrium_Brutal_Specular.png`
- `output/CorypheusRedLyrium_Brutal_Specular.dds`
- `output/CorypheusRedLyrium_Brutal_Emissive.png`
- `output/CorypheusRedLyrium_Brutal_Emissive.dds`

Quick start:
1. Install Python 3.11+
2. `pip install -r requirements.txt`
3. `python generate_red_lyrium.py`
4. Open the generated files and export/import them into your DA2 asset pipeline.

For an actual DA2 ERF:
- You need the original game asset package and the modding tool used for your DA2 installation.
- Once the exact texture asset path and original swap target are known, the generated DDS files can be placed into the correct asset tree and packed into ERF using your DA2 toolchain.

This project is intended as a solid base for the Corypheus red lyrium look and must be adapted to the exact original armor UV/asset before being shipped as a game-ready mod.
