# Braço robótico de 6 GDL (EB-15)

Braço robótico de 6 graus de liberdade baseado no atuador Robotic Actuator EB-15. A cinemática e a dinâmica são representadas com a biblioteca Robotics Toolbox for Python.

## Estrutura
- `STLs/`: peças do braço para impressão 3D.
- `Fatiado/`: arquivos fatiados (`3MS/` com os `.3mf` e `Gcode/` com os G-codes do corpo e das engrenagens).
- `Hardware/Wokwi/`: simulação no Wokwi do ESP32 com 6 drivers de passo, 6 motores e 6 encoders MT6701 (ver `LEIA-ME.md` da pasta).
- `Robotics-Arm-EB-15-main/`: desenhos de montagem e licença do atuador EB-15 (material do fabricante, https://toolboxrobotics.com/robotic-arm-eb15).
- `Testes-RoboticsToolbox/`: primeiros testes de cinemática com a biblioteca (modelo Panda e trajetória em forma de coração no notebook, scripts `Teste.py`, `Teste2.py`, `teste3.py` e `python-project1/`).

## Como executar
- Python: `pip install roboticstoolbox-python` (ou `pip install -r Testes-RoboticsToolbox/python-project1/requirements.txt`) e rodar os scripts.
- Simulação: abrir `Hardware/Wokwi/` no Wokwi, como descrito no `LEIA-ME.md` da pasta.
