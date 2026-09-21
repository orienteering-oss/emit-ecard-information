# EMIT e-card information

This repository collects public information and teardown photographs for the EMIT electronic punching card used in orienteering.

The exterior photograph shows card number `118553` and the separate text `06 10`.
The repository does not establish what `06 10` means or which e-card hardware version is pictured.

## Current public information

Emit currently sells [Ver.5](https://emit.no/en/nettbutikk/loperbrikke-ver-5/) and [Ver.7](https://emit.no/en/nettbutikk/loperbrikke-ver-7/) e-cards.
Emit describes Ver.7 as its newest e-card and says that it replaces Ver.6.
The linked product pages say that both versions store up to 50 times until reset at a start unit.

The product photographs and descriptions do not establish that the board pictured in this repository is electrically identical to either current product.

## Teardown photographs

![Outside of the opened e-card](./emit-ecard-outside.jpg)

![Inside of the e-card housing](./emit-ecard-inside.jpg)

![Circuit board in the housing](./emit-ecard-inside-circuit-board.jpg)

![Circuit board component side](./emit-ecard-circuit-board-front.jpg)

![Circuit board reverse side](./emit-ecard-circuit-board-back.jpg)

![Circuit board component side, alternate view](./emit-ecard-circuit-board-front2.jpg)

## Research notes

- [Confirmed markings and datasheets](./docs/components.md) records only text that can be read from the photographs.
- [Public documents and known gaps](./docs/research-status.md) separates published facts from the evidence still needed for a schematic or board model.

## Reconstruction status

This repository does not yet contain physical dimensions, a schematic, a PCB layout, a netlist, firmware, coil measurements, or captures of the card-to-unit communication.
A board model made from the current photographs would therefore be speculative and has not been added.
