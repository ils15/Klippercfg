<div align="center">

# 🖨️ 3D Printers Configurations

[![Klipper](https://img.shields.io/badge/klipper-configs-blue?style=flat-square&logo=github&logoColor=white)](https://www.klipper3d.org/)

_Configurações específicas para diferentes modelos de impressoras 3D_

</div>

## 🇧🇷 Português

Esta pasta contém configurações específicas para diferentes modelos de impressoras 3D, facilitando a migração para o Klipper.

### 📁 Estrutura

As configurações estão organizadas de forma hierárquica:

```
3D Printers config/
├── Fabricante/
│   ├── Modelo/
│   │   ├── printer.cfg
│   │   ├── macros.cfg
│   │   └── README.md
```

Exemplos:
- Creality/Ender 3/
- Prusa/Mini/
- Voron/2.4/

### 📋 Como Usar

1. Navegue até a pasta do modelo da sua impressora
2. Revise os arquivos de configuração disponíveis
3. Copie os arquivos para a pasta de configuração do seu Klipper
   ```bash
   cp -r "3D Printers config/Fabricante/Modelo/*" ~/printer_data/config/
   ```
4. Adapte os arquivos para suas necessidades específicas
   - Verifique os pinos MCU
   - Ajuste dimensões da impressora
   - Configure os endstops e sensores

### 💡 Klipper vs. Firmwares Tradicionais

| Aspecto | Klipper | Marlin/RepRap |
|---------|---------|--------------|
| **Processamento** | No computador (Pi) | No microcontrolador |
| **Atualizações** | Sem reflash | Requer reflash |
| **Interface** | Web (Mainsail/Fluidd) | LCD/Web separado |
| **Recursos avançados** | Input Shaping, PA | Limitados por hardware |
| **Múltiplos MCUs** | Suportado nativamente | Complexo/Impossível |

### 🤝 Contribuindo

Ao adicionar configurações para uma nova impressora:
- Crie uma pasta com o nome do fabricante, se ainda não existir
- Dentro dela, crie uma pasta com o modelo da impressora
- Adicione arquivos de configuração bem documentados:
  - `printer.cfg` - Configuração principal
  - `macros.cfg` - Macros específicas da impressora
  - `README.md` - Notas sobre particularidades da impressora
- Inclua informações sobre quaisquer modificações ou configurações de hardware específicas

---

## 🇬🇧 English

This folder contains specific configurations for different 3D printer models, facilitating the migration to Klipper.

### 📁 Structure

The configurations are organized in a hierarchical way:

```
3D Printers config/
├── Manufacturer/
│   ├── Model/
│   │   ├── printer.cfg
│   │   ├── macros.cfg
│   │   └── README.md
```

Examples:
- Creality/Ender 3/
- Prusa/Mini/
- Voron/2.4/

### 📋 How to Use

1. Navigate to your printer model's folder
2. Review the available configuration files
3. Copy the files to your Klipper configuration folder
   ```bash
   cp -r "3D Printers config/Manufacturer/Model/*" ~/printer_data/config/
   ```
4. Adapt the files to your specific needs
   - Verify MCU pins
   - Adjust printer dimensions
   - Configure endstops and sensors

### 💡 Klipper vs. Traditional Firmwares

| Aspect | Klipper | Marlin/RepRap |
|--------|---------|--------------|
| **Processing** | On computer (Pi) | On microcontroller |
| **Updates** | No reflash | Requires reflash |
| **Interface** | Web (Mainsail/Fluidd) | LCD/Separate web |
| **Advanced features** | Input Shaping, PA | Limited by hardware |
| **Multiple MCUs** | Natively supported | Complex/Impossible |

### 🤝 Contributing

When adding configurations for a new printer:
- Create a folder with the manufacturer's name, if it doesn't exist yet
- Inside it, create a folder with the printer model
- Add well-documented configuration files:
  - `printer.cfg` - Main configuration
  - `macros.cfg` - Printer-specific macros
  - `README.md` - Notes about printer particularities
- Include information about any specific hardware modifications or settings

---

<div align="center">
<b>Klipper - https://www.klipper3d.org/</b>
</div>
