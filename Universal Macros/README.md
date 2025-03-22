# Universal Macros

## 🇧🇷 Português

Esta pasta contém macros universais que podem ser utilizadas em praticamente qualquer impressora 3D que use o firmware Klipper.

### Estrutura de Arquivos

- **macros.cfg**: Arquivo principal que inclui todos os outros arquivos de macros
- **conditional_homing.cfg**: Macros para homing condicional
- **pause_resume_cancel.cfg**: Macros para pausar, retomar e cancelar impressões
- **bed_mesh.cfg**: Macros para mapeamento da cama
- **tuning.cfg**: Macros para ajuste e calibração
- **utility.cfg**: Macros utilitárias diversas
- **filament.cfg**: Macros relacionadas ao gerenciamento de filamento
- **start_end_macros.cfg**: Macros para início e fim de impressão

### Como Usar

1. Copie os arquivos desejados para sua pasta de configuração do Klipper
2. Inclua-os no seu arquivo `printer.cfg` usando `[include macros/nome_do_arquivo.cfg]` ou inclua apenas o arquivo `macros.cfg` que referenciará todos os outros
3. Reinicie o Klipper para aplicar as alterações

### Contribuindo

Ao adicionar novas macros, certifique-se de:
- Documentar claramente o propósito da macro
- Explicar os parâmetros utilizados
- Indicar quaisquer dependências ou requisitos especiais
- Adicionar a macro ao arquivo apropriado com base em sua funcionalidade

---

## 🇬🇧 English

This folder contains universal macros that can be used on virtually any 3D printer running the Klipper firmware.

### File Structure

- **macros.cfg**: Main file that includes all other macro files
- **conditional_homing.cfg**: Macros for conditional homing
- **pause_resume_cancel.cfg**: Macros for pausing, resuming, and canceling prints
- **bed_mesh.cfg**: Macros for bed mapping
- **tuning.cfg**: Macros for adjustment and calibration
- **utility.cfg**: Various utility macros
- **filament.cfg**: Macros related to filament management
- **start_end_macros.cfg**: Macros for print start and end

### How to Use

1. Copy the desired files to your Klipper configuration folder
2. Include them in your `printer.cfg` file using `[include macros/filename.cfg]` or just include the `macros.cfg` file which will reference all others
3. Restart Klipper to apply the changes

### Contributing

When adding new macros, make sure to:
- Clearly document the purpose of the macro
- Explain the parameters used
- Indicate any dependencies or special requirements
- Add the macro to the appropriate file based on its functionality
