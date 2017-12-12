# Project Scaffolding


## Project Folders
| Folder | Purpose |
| --- | --- |
| config | Settings for bundling/deployment the package |
| dist |	Final code files which are distributed with your application |
| lib |	Processed code files which are ready to move into the bundle |
| node_modules |JS modules used by the solution |
| sharepoint | Default folder where the package/asset is exported |
| src |	Where you structure/write the code solution |
| typings |	TypeScript typings |


### Scaffolding SRC folder
Below is described the best way to scaffold the source folder where all folders and files of your SPFx solution are going to live.

    ....
    ├── src
    │   │── webparts
    │   │   ├── MyCustomWebpart
    │   │   │   ├── MyCustomWebpart.ts
    │   │   │   ├── data
    │   │   │   ├── loc
    │   │   │   ├── models
    │   │   │   ├── styles
    │   │   │   ├── tests
    │   │   │   ├── components
    │   │   │   │   ├── ComponentName
    │   │   │   │   │   ├── ComponentName.tsx
    │   │   │   │   │   ├── IComponentNameProps.ts
    │   │   │   │   │   ├── IComponentNameState.ts
    │   │   │   │   │   ├── index.ts
    │   │   │   │   │   ├── ComponentName.test.ts
    │   │   │   │   │   └── styles.module.scss
    │   │   │   │   ├── AnotherComponent
    │   │   │   │   │   ├── ...
    ....

Each folder/file purpose is described below:
| Folder/File | Purpose |
| --- | --- |
| MyCustomWebpart.ts | Initial file that will instantiate the render of the webpart and manage its configuration panel settings |
| data | To store api calls |
| loc | To store localization strings |
| models | To store the models of the objects to use on your webpart code |
| styles | To store global styles and variables of the SCSS of the webpart |
| tests | To store global tests of the webpart |
| components | To store all the components that integrate the webpart |
| ComponentName | <ul><li>Folder and component name files should be in PascalCase format </li><br />Each component folder should contain its corresponding:<li>Index file to export modules</li><li>Component file to declare the functionality of the component</li><li>Interface files to declare the props and state of the component</li><li>Testing unit file</li><li>Styles file</li></ul> |


## Resources
### Tutorials

  * [Recommendations for working with CSS in SharePoint Framework solutions](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/css-recommendations)

### References
  * [Scaffold projects using yeoman SharePoint generator](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/toolchain/scaffolding-projects-using-yeoman-sharepoint-generator)

## Next chapter
  * [APIs](./APIs)
