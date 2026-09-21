# Public documents and known gaps

## Official product information

Emit's current [Ver.5 product page](https://emit.no/en/nettbutikk/loperbrikke-ver-5/) states that the card stores up to 50 times, remains active for six hours after the previous punch, and operates from -20 °C to +50 °C.
Emit's current [Ver.7 product page](https://emit.no/en/nettbutikk/loperbrikke-ver-7/) describes Ver.7 as the newest card, says it replaces Ver.6, and states that its LED flashes for five seconds after a punch.
Emit's [2022 product overview](https://emit.no/wp-content/uploads/2022/09/Emit-products-orienteering-2022.pdf), also available as a [local copy](../emit-products-orienteering-2022.pdf), says the original system was introduced in 1994, Ver.5 electronics were updated in 2015, and Ver.6 was introduced in 2016.

These sources describe product behavior and compatibility.
They do not publish the card schematic, PCB files, firmware, memory map, or card-to-unit physical protocol.

## Reader protocol document

Emit publicly serves an [eScan2 USB command protocol PDF](https://emit.no/wp-content/uploads/2021/03/ESCAN2-protocol-specification-V1.0.pdf).
The document says that it describes USB communication with the eScan2 and includes an e-card output-frame format.
It does not claim to describe the physical communication between an e-card and a control unit.

The PDF also labels itself confidential and says that reproduction or disclosure is not allowed without authorization.
This repository therefore links to the vendor-hosted copy and does not mirror it.

## Evidence required before creating a board model

The following items are absent from the repository and require measurements from hardware.

- Caliper measurements of the bare PCB outline, thickness, cutouts, and component locations.
- Perpendicular, calibrated scans or photographs of both sides of a cleaned board.
- PCB layer count, copper thickness, trace widths, via sizes, and continuity measurements.
- Inductance, resistance, quality factor, and connection details for each spiral trace structure.
- Exact identification and electrical values for every component.
- A traced schematic and checked netlist.
- Firmware or a documented replacement implementation.
- Captures and documentation of control, start, and reader communication with the card.
- EEPROM contents from controlled before-and-after experiments to establish the memory format.

Until those measurements exist, a KiCad, Gerber, STEP, or OpenSCAD file would encode guesses rather than recover the original board.

## Practical next step

The most useful next contribution is a measurement record from one sacrificial card.
It should identify the card version if known and include unambiguous photographs, board dimensions, component markings, continuity results, and coil measurements.

Any experimental implementation should be kept out of event use until compatibility, safety, and the applicable [IOF approval requirements](https://orienteering.sport/iof/it/electronic-punching/) have been addressed.
