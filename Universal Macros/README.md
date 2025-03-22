<div align="center">

# 🔧 Universal Macros

[![Klipper](https://img.shields.io/badge/klipper-compatible-blue?style=flat-square&logo=github&logoColor=white)](https://www.klipper3d.org/)

_Macros universais para qualquer impressora 3D com Klipper_

</div>

## 🇧🇷 Português

Esta pasta contém macros universais que podem ser utilizadas em praticamente qualquer impressora 3D que use o firmware Klipper.

### 📁 Estrutura de Arquivos

| Arquivo | Descrição |
|---------|-----------|
| **macros.cfg** | Arquivo principal que inclui todos os outros arquivos de macros |
| **conditional_homing.cfg** | Macros para homing condicional, garantindo que seus eixos estejam sempre na origem quando necessário |
| **pause_resume_cancel.cfg** | Macros para pausar, retomar e cancelar impressões com gestão inteligente de filamento |
| **bed_mesh.cfg** | Macros para mapeamento da cama, calibração e compensação automática |
| **tuning.cfg** | Macros para ajuste e calibração de parâmetros como pressure advance e input shaping |
| **utility.cfg** | Macros utilitárias diversas para simplificar operações comuns |
| **filament.cfg** | Macros relacionadas ao gerenciamento de filamento, incluindo troca e purga |
| **start_end_macros.cfg** | Macros para início e fim de impressão, garantindo uma correta preparação e finalização |

### 📋 Como Usar

1. Copie os arquivos desejados para sua pasta de configuração do Klipper
   ```bash
   cp -r Universal\ Macros/*.cfg ~/printer_data/config/macros/
   ```
2. Inclua-os no seu arquivo `printer.cfg` usando:
   ```
   [include macros/nome_do_arquivo.cfg]
   ```
   Ou inclua apenas o arquivo `macros.cfg` que referenciará todos os outros:
   ```
   [include macros/macros.cfg]
   ```
3. Reinicie o Klipper para aplicar as alterações:
   ```bash
   ~/klippy-env/bin/python ~/klipper/scripts/helprs/update_manager.py restart
   ```

### 💡 Exemplos de Uso

```gcode
# Exemplo de uso da macro de início de impressão
START_PRINT BED=60 EXTRUDER=210

# Exemplo de macro para troca de filamento
FILAMENT_CHANGE
```

### 🤝 Contribuindo

Ao adicionar novas macros, certifique-se de:
- Documentar claramente o propósito da macro
- Explicar os parâmetros utilizados
- Indicar quaisquer dependências ou requisitos especiais
- Adicionar a macro ao arquivo apropriado com base em sua funcionalidade
- Incluir comentários explicativos dentro do código

---

## 🇬🇧 English

This folder contains universal macros that can be used on virtually any 3D printer running the Klipper firmware.

### 📁 File Structure

| File | Description |
|------|-------------|
| **macros.cfg** | Main file that includes all other macro files |
| **conditional_homing.cfg** | Macros for conditional homing, ensuring your axes are always home when needed |
| **pause_resume_cancel.cfg** | Macros for pausing, resuming, and canceling prints with smart filament management |
| **bed_mesh.cfg** | Macros for bed mapping, calibration, and automatic compensation |
| **tuning.cfg** | Macros for adjustment and calibration of parameters like pressure advance and input shaping |
| **utility.cfg** | Various utility macros to simplify common operations |
| **filament.cfg** | Macros related to filament management, including change and purge |
| **start_end_macros.cfg** | Macros for print start and end, ensuring proper preparation and finalization |

### 📋 How to Use

1. Copy the desired files to your Klipper configuration folder
   ```bash
   cp -r Universal\ Macros/*.cfg ~/printer_data/config/macros/
   ```
2. Include them in your `printer.cfg` file using:
   ```
   [include macros/filename.cfg]
   ```
   Or just include the `macros.cfg` file which will reference all others:
   ```
   [include macros/macros.cfg]
   ```
3. Restart Klipper to apply the changes:
   ```bash
   ~/klippy-env/bin/python ~/klipper/scripts/helprs/update_manager.py restart
   ```

### 💡 Usage Examples

```gcode
# Example of using the print start macro
START_PRINT BED=60 EXTRUDER=210

# Example of filament change macro
FILAMENT_CHANGE
```

### 🤝 Contributing

When adding new macros, make sure to:
- Clearly document the purpose of the macro
- Explain the parameters used
- Indicate any dependencies or special requirements
- Add the macro to the appropriate file based on its functionality
- Include explanatory comments within the code

---

<div align="center">
<b>Klipper - https://www.klipper3d.org/</b>
</div>
