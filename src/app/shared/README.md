This folder and NgModule should contain all elements of the application that are intended to be used across multiple feature modules. This module will get imported into all application feature modules. This should **NOT** contain services or files associated with services (Interface files, Redux, etc.). Contents should include:
- Components
- Directives
- Pipes

Files should be broken down into descriptive folders in order to allow for quick lookup of the appropriate file. Options may include:
- form
- validators
- layout
- etc...

Elements could also be broken down into separate NgModules if desired (like when dealing with an organization-wide component library). Most of the time, further module breakdown is unneeded and could impose a negative cognitive overhead.