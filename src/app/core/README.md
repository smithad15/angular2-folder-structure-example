This folder and NgModule should contain all global service-related elements. This module should only be imported into the root AppModule. This should **NOT** contain any UI related elements like components, directives, or pipes. Contents should include:
- Global singleton services
- Feature services that are used across feature modules

Feature services that are used across feature modules should be moved from their top level feature folder into a feature-labeled subfolder inside this module. This will ensure that you do not have any Dependency Injection bugs if you choose to lazy-load your feature modules through the router.