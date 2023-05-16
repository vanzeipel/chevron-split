# chevron-split
A split, column-staggered mechanical keyboard where the key layout forms something of a chevron shape that more closely follows the natural resting position of the fingers. 52-key layout with 3 thumb keys and a rotary knob on the right half. Uses the Pro Micro Elite-C controller as the primary controller and any compatible Pro Micro as the secondary controller on the other half.

## Getting Started
All the files you'll need to fabricate the keyboard's PCB and 3D printed case are included in the `/pcbs` and `/cases` directories. You can use them to print your 3D case and upload the BOM to get a PCB printed.

### Making Layout Changes
If you want to make any adjustments to the layout, you'll need to generate new outlines and PCB files.

### Setup
1. Make sure Node.js Package Manager `npm` is installed.
2. Run `npm install` to install the required packages defined in `package.json`.
3. Run `npm run patch-footprints` to make the custom PCB component footprints available to the local `ergogen` package.

### Rebuilding the Layout
1. Modify `/layout/config.yaml`
2. Run `npm run gen` to invoke `ergogen` on the `/layout/config.yaml` to build the outlines and basic PCB files, located in the `/output` directory.