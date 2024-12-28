# My KiCad Libraries

This repository contains shared libraries and resources for use with KiCad projects.
It includes official KiCad libraries, DigiKey libraries, and custom symbols, footprints, and templates for hardware design.

## Repository Structure

```
My_KiCad_Libraries/
├── kicad-symbols/                     # Submodule: Official KiCad symbols
├── kicad-footprints/                  # Submodule: Official KiCad footprints
├── kicad-packages3d/                  # Submodule: Official KiCad 3D models
├── custom_symbols/                    # Custom schematic symbols
│   ├── MySerialParts.lib
│   ├── MySerialParts.dcm
│   └── README.md
├── custom_footprints/                 # Custom footprints
│   ├── DIP_Probing_Interfaces.pretty/
│   │   ├── Probe_Header.kicad_mod
│   │   ├── Oscilloscope_Pin.kicad_mod
│   └── README.md
├── templates/                         # Project templates for reuse
│   ├── Probing_Interface_Template.kicad_sch
│   ├── USB_Console_Interface_Template.kicad_sch
│   └── README.md
└── .gitmodules                        # Submodule definitions
```

## Getting Started

### Clone the Repository

To use these libraries, clone the repository with submodules:

```bash
git clone --recurse-submodules https://github.com/yourusername/My_KiCad_Libraries.git
```

### Submodule Initialization

If you've already cloned the repository without submodules, initialize and update them with:

```bash
git submodule update --init --recursive
```

## Usage

- **Symbols and Footprints**: Point KiCad to the appropriate directories in this repository (e.g., `kicad-symbols` and `custom_footprints`) using the **Library Manager**.
- **Templates**: Copy templates from the `templates` directory into your project as needed.

## Updating Submodules

To update the submodules to their latest versions, run:

```bash
git submodule update --remote
git commit -am "Updated submodules to latest upstream versions"
```

## Contributing

Feel free to contribute custom symbols, footprints, or templates that might be useful for other hardware designers.
Open a pull request with your additions or improvements.

## License

This repository includes:
- **Submodules**: Licensed as per their respective repositories (e.g., KiCad libraries).
- **Custom Content**: Licensed under [Creative Commons Attribution-NonCommercial 4.0 International (CC BY-NC 4.0)](https://creativecommons.org/licenses/by-nc/4.0/).

Please ensure compliance with the licenses of individual components.
```

---

### **Customizations**
1. Replace `https://github.com/yourusername/My_KiCad_Libraries.git` with the actual repository URL.
2. Adjust the licensing section if you decide to use a different license for your custom content.

Let me know if you need further tweaks!