# RobotMechanics
A repository for the Mechanics Team of the project. It includes robot 3D models, simulations and documentation of mechanical components.


## Solidworks file problems
If there are any problems with assembly file not seeing the part files while opening click on **find part** and then file the folder in which the part file should be. Solidworks will automatically fix the part reference.

## Toolbox File Imports
Please when using the solidworks base files save them to the repo so that everyone using the project has all the parts necessary to open all the files.

## GIT - LFS
### To add a file to git LFS (Large File Storage):
	1. `git lfs track "*.<rozszerzenie pliku>"` np. `git lfs track "*.jpeg"`
	2. `git lfs migrate`
	3. `git push`

	
	
### To block and unlock files from simultaneous modification:
**Blocking modifiaction** - `git lfs lock <file-path>`
**Unlocking** -  `git lfs unlock <file-path>`
**Check which files are locked** - `git lfs locks`

## Repo Usage
### Folder Structure
- 3d Models
	- Materials
	- Drawing templates
	- Parts and Subassemblies
		- Assembly specific
			- [Example] Front Right Leg (Here there is no project version because components are shared between assembly versions)
				- 3D Printed
					- "Link A - v0 2024 09 11 - elongated"
					- Link B Parts
					- "Link B - v2 2024 01 12  - assembled"
	- Components
			- Mechanical
				- "Servo holder (abcd123) - v0 24 11 09"
			- Electrical
			- Fasteners
				- "Screw 10mm x 2mm flat head - 24 09 01"
	- Projects
		- Project Archive (here we throw unused old projects that are obsolete)
		- PROJECT TEMPLATE (For copying)
			- Assemblies
			- ...
		- ... Front Right Leg - v0
			- Assemblies
			- Drawings
			- Documentation
			- Simulations
			- Miscelanous
- Robot Documentation


### File Name structure 
**Project** - "project name - v**x**". - A big thing to do (e.g. Changing the structure of a leg with new parts and different dimensions). If there is already a leg "v0" then the next leg will be called "v1". Projects do not have to be related to modeling. For example a project can be a calculation of centers of gravity of segments

**Assemblies, Subassemblies Parts etc** - "Name (part number if bought) - version number Year month day - notes if any". 
- For example
	- "Link A - v0 2024 09 11 - elongated".
	- "Servo 130kg (abc36A51) - v1 2025 11 09 - weight accurate to model bought "

**Small bought parts** - "Name (part number if bought)" - Part models that are unlikely to change, for example a specific screw model or a magnet with pre defined dimensions, can be made without a Version Number.

### General Usage Notes
- Please add organising folders if needed, the folder tree shows only where various files should exist and not how to exactly manage them in those places

- If there are any questions or a file can have various name structures please use one that gives more information, not less. It is better to add a version number and not need it later that to add this information later on.

- If you have any suggestions or improvments to the File Managment System please write about it or get in touch. This system should evolve with the projects. If something is bothering you with the structure or naming scheme please **raise an issue or contact NimbleStatic directly**.
