## What’s hold in this repository?
This repository will hold all the information about the Mechanics of the BCN3D Sigma.
As a declared Open Source organization, it's in our mission to release all the original design files to you to be able to learn, reuse and improve. Open Source not only means code, it also concerns hardware.

We’ve managed to design and manufacture the BCN3D Sigma thanks to our previous experience in the 3D printing industry, the ideas coming from the community, our engineering background and a narrow collaboration with our suppliers. Our goal is justify the decisions we took and share the know-how we acquired so far.

We also provide the source files for those who want to check the core of the BCN3D Sigma. You can consult both the CAD files and the technical drawings.

## CONCEPT DESIGN
During the concept design stage we set a clear target which determined the whole design and decisions: The BCN3D Sigma is a professional printer.

### Aesthetics
It has to look  like a professional equipment. Our previous printers were made with aluminium extruded profiles and plastic printed parts. That made sense for printers oriented to makers or schools, sold as a kit. But, in this case, aesthetic was a major player. For this reason, we adopted a welded aluminium frame, which allows the Sigma to be a unique and attractive 3D printer

### Multimaterial
As a professional printer, it has to print as many materials as possible. Not only for engineers, who require tough -or flexible-, functional polymers, but also for designers who need the aesthetic component. However, material is not the only limitation. Complex geometries, overhangs and 3D printing doesn’t get along. So we wanted the Sigma to be a real solution for those users who need to print with supports as a must. In conclusion, the Sigma is the first and only commercial 3D printer with an Independent Dual Extuder (IDEX) system, which avoid all the side problems dual extrusion may cause.

### High Quality
The 3D Printing industry is maturing. Users are more and more demanding and 3D printing must be a solution, not a headache. For this reason, the Sigma has to be a reliable piece of engineering, easy to assemble, maintain and capable to print seamlessly high quality objects, no matter how complex they are.

### High Capacity
Real-life and functional parts are not always small. A big printing volume is a great advantage for a professional 3D Printer although the Sigma intends to be a desktop-sized printer. Allocating all the items and devices inside the frame, while granting ease-to-use and optimizing the axes structure were a key goal.

## DETAIL DESIGN INSIGHTS

We faced dozens of challenges during the design process. Below we describe some of them:

### Frame
Probably the biggest challenge. First we thought in a chassis made of profiles and then cover it. But then realized the cost in materials for that solution would be high enough to look for alternatives that could contribute more in the aesthetic field, even that could be a bit more expensive. On the other side, we wanted the Sigma to be an accessible printer, wide and open in order to ease the handling and operation. So we decided to explore the option of designing a unibody frame where all the mechanical components were mounted on and with a wide frontal oberture.

First we had to decide between using aluminium or steel. Steel offers many advantages: It’s a very stiff metal, great to build structures and precise mechanical systems. In addition, it’s easy to work with and cheap. But it’s -really- heavy. We contemplated the option of using a thinner metal sheet of steel for the frame. After ordering a prototype, we dismissed the idea, though. Still it had a great mechanical behaviour and a relative low weight, the feeling of touching a thin metal sheet (1.5mm) was unpleasant because it felt like a cutting edge. And it didn’t look sturdy. So to achieve both a reliable look and a pleasant contact, we needed to go up to 3mm thickness. But then the shipping costs would be absurdly high and the handling, a constant hassle -both during the assembly process and for the final user.

Aluminium, on the other hand, provides lightness and a smooth and sturdy look. But it’s more expensive as a material and it’s harder to laser cut and weld. After balancing pros and cons, we bet on aluminium option -although we had a plan B.

The second big issue to manage was the manufacturing process. We contemplated two different ways to do it: either manufacture the frame by parts and screw them all together in the assembly line or weld the frame. Welding aluminium is hard and the welding process itself has some thermal and geometric implications that have to be considered. But it allows to reduce the assembling time dramatically while it outsources a key process.

As alternative, designing the frame as separate parts to screw together was considerably cheaper - as you save a handmade process such as welding and polishing. But the assembling of the frame and adjustment could be very delicate and incompatible with our production tag time. So the overall cost wouldn’t be that different in both options. The aesthetic component, though, would be very penalized with this alternative, because we would need to add dozens of screws on the frame.

For these reasons, we finally opted for a welded structure. We sat hours with our supplier discussing the best way to design every single part in order to grant a proper alignment between the faces that would hold the axes. Furthermore, we also studied the mechanical behaviour of the frame with some CAE studies, simulating stress and deformations during a standard usage.

### High quality components
A good frame is not enough to achieve amazing results. In such a precision equipment as the Sigma, all the mechanical components play a key role. Due to the product requirements in terms of size and use of the internal space of the printer we had, we opted for a axes structure with the toolheads moving in the XY plane and an up and down moving Z axis.

With the XY plane decided to mount high precision linear guides. Despite its cost slightly higher than a system based on rods and bearings, the linear rails offer a professional look, an easy assembling and a compact package.

Regarding the Z axis, we were aware of the importance to have a robust guide system in order to avoid classic artifacts in printed parts related with a bad Z performance, such as Z wobbling. We also had experience using couplings and to connect the actuator with the leadscrew and we knew that a bad assembling could cause poor quality results. With this background, we chose using Ø12mm guide rods and a stepper motor with an inserted leadscrew. The whole system provides a high repeatability and accuracy.

### Independent Dual Extrusion
A 3D printer with such an specific feature increases the design unknowns and multiplies the components. Not only the firmware and the electronics need to be highly customized, but also mechanically there are some decisions to take.

First of all, because of the multiple components to hold, the internal parts tend to be more complex than other printers. So we decided to use aluminium sheet bending technology to manufacture the inner parts. As the manufacturing tolerances are acceptable for the purposes we intend and the technology is cheap and easily scalable, we considered the technology optimum.  

Two independent Extruders means have an extra moving stepper for the second toolhead, and the extra toolhead itself. On the other hand, when printing with both extruders it’s important to have a bucket to purge the idle hotends before start printing the model again. All this parts add weight to a moving element, which is a problem to print fast because the high inertias may worsen the print quality. So we designed the X and Y Axis as light as possible, saving as many grams as possible with every single component. Not only weight is important when doubling the toolheads, but also space. So we decided to adopt a bowden-based feeding system and miniaturize all the items as much as possible.

### Big Printing Volume
The BCN3D Sigma features 210x297x210mm printing volume. In order to provide such a big volume and a free space on both sides to park the idle toolhead, but still having a desktop-sized printer, we had to reorient the Z platform. The main issue to solve, though, was granting the stiffness of the structure with a big overhang of more than 300mm.

To prevent vibrations, we adopted high quality bearings with low clearance and we designed and  simulated a custom metal sheet structure, which allows to get a great quality prints with a smooth surface despite the big overhang.
