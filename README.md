# Assembler
Vorlesung über Assemblerprogrammierung (32 Lehrveranstaltungsstunden)

## Inhalte
- Grundlagen Mikroprozessortechnik
- Aufbau von Mikroprozessoren
  - Komponenten
  - Bussysteme
  - Prozessorarchitekturen
  - Herstellungsprozess
  - Bautypen
- Assemblerprogrammierung

# Grundlagen Mikroprozessortechnik – Stichworte

## Architektur
- **Von-Neumann-Architektur**: gemeinsamer Daten-/Programmspeicher, sequenzielle Verarbeitung
- **Harvard-Architektur**: getrennter Daten- und Programmspeicher für höhere Effizienz
- **RISC vs. CISC**: reduced vs. complex instruction set
- **Registersatz**: Arbeitsregister, Akkumulator, Indexregister

## Grundkomponenten
- **ALU** (Arithmetic Logic Unit): Rechenwerk für arithmetische & logische Operationen
- **CU** (Control Unit): Steuerwerk, Befehlsdekodierung, Koordination Befehlsausführung und Datenfluss
- **PC** (Program Counter): Befehlszähler
- **SP** (Stack Pointer): Stapelzeiger
- **IR** (Instruction Register): aktueller Befehl
- **MAR / MDR**: Adress- / Datenregister des Speichers
- Register: Temporärer Specher für Daten und Adressen
- Cache: Schneller Zwischenspeicher zur Optimierung der Leistung

## Bus-System
- **Adressbus**: unidirektional, bestimmt Adressraum (2ⁿ Adressen bei n Bit)
- **Datenbus**: bidirektional, Busbreite = Wortbreite
- **Steuerbus**: R/W, Clock, Reset, IRQ …
- Busbreite
- Busprotokolle

## Befehlszyklus (Fetch–Decode–Execute)
1. **Fetch**: Befehl aus Speicher holen (PC → MAR → IR)
2. **Decode**: Opcode auswerten
3. **Execute**: Operation ausführen, PC inkrementieren

## Befehlsverarbeitung
- Maschinenbefehle (Instrution Set)
- Opcode
- Operanden
- Fetch-Decode-Execute-Zyklus (Verarbeituzng binärer Anweisungen im Mikroprozessor)
- Pipeline

## Adressierungsarten
- Unmittelbar (Immediate)
- Direkt / Indirekt
- Register / Registerindirekt
- Relativ / Indiziert

## Speicher
- **RAM** (Random Access Memory: SRAM / DRAM): flüchtig, Arbeitsspeicher
- **ROM (Read Only Memory) / Flash / EEPROM**: nichtflüchtig, Programmspeicher
- **Cache**: L1/L2/L3, Lokalitätsprinzip
- **Speicherhierarchie**: Register → Cache → RAM → Flash/HDD
- Speicheradressierung

## Interrupts & Ausnahmen
- **IRQ** (Interrupt Request): externe/interne Unterbrechung
- **ISR** (Interrupt Service Routine)
- **Interrupt-Vektor-Tabelle**
- **NMI** (Non-Maskable Interrupt)
- **Polling vs. Interrupt**: aktives Warten vs. ereignisgesteuert

## Takt & Timing
- **Taktfrequenz / Taktperiode**
- **CPI** (Cycles per Instruction)
- **MIPS** (Millions of Instructions per Second)
- **Pipeline**: IF – ID – EX – MEM – WB; Hazards (Daten-, Steuer-, Strukturhazard)
- Clock-Signal
- Zykluszeit
- Synchronisierung

## Ein-/Ausgabe (I/O)
- **Memory-mapped I/O** vs. **Port-mapped I/O**
- **GPIO** (General Purpose I/O)
- **DMA** (Direct Memory Access): busmastering ohne CPU
- Serielle Schnittstellen: UART, SPI, I²C
- Interrupts
- Polling
- Peripherie

## Programmierung
- Assembler
- Maschinensprache
- Hochsprachen (z.B. C)
- Cross-Compiler
- Debugging

## Mikrocontroller vs. Mikroprozessor
| | Mikroprozessor | Mikrocontroller |
|---|---|---|
| CPU | extern ergänzt | integriert |
| Peripherie | extern | on-chip (Timer, ADC, …) |
| Einsatz | allgemein (PC) | eingebettete Systeme |

## Mikrocontroller-Peripherie
- Timer/Counter
- ADC (Analog-Digital-Wandler)
- DAC (Digital-Analog-Wandler)
- UART / SPI / I²C
- GPIO

## Typische Kenndaten
- Wortbreite: 8 / 16 / 32 / 64 Bit
- Adressraum: 2ⁿ Byte
- Versorgungsspannung: 1,8 V – 5 V
- Befehlssatz: Anzahl Opcodes, Befehlsformat (1–4 Byte)

## Lost&Found

- Prozessor (CPU)
- Embedded Systems
- Akkumulator
- Interrupt-Prioritäten
- Echtzeitsysteme
- Energieverbrauch/Low-Power-Modes
- Hardware-Software-Co-Design
- Systembus verbindet Prozessor, Speicher und Peripherie
- Interrupts ermöglichen reaktive Programmierung
