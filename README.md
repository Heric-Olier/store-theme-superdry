# Store Theme Superdry

![All Contributors](https://img.shields.io/badge/all_contributors-1-orange.svg?style=flat-square)

<Julio Colombia> Store Theme is basic store front model based on the VTEX IO Store Framework.
## Preview
![](https://i.imgur.com/QYi27RB.jpg)
### Step 1 - Basic setup

Access the VTEX IO [basic setup guide](https://vtex.io/docs/getting-started/build-stores-with-store-framework/1) and follow all the given steps.

By the end of the setup, you should have the VTEX command line interface (Toolbelt) installed along with a developer workspace you can work in.

### Step 2 - Cloning the Minimum Boilerplate Theme repository

Clone this [template](https://help.github.com/en/github/creating-cloning-and-archiving-repositories/cloning-a-repository) repository to your local files to be able to effectively start working on it.

Then, access the repository's directory using your terminal.

### Step 3 - Editing the Manifest.json

Once in the repository directory, it is time to edit the Minimum Boilerplate manifest.json file.

Once you are in the file, you must replace the vendor and account values. 

Vendor is the account name you are working on and account is anything you want to name your theme. For example:

```json
{
  "vendor": "store",
  "name": "store-theme",
}
```
### Step 4 - Installing required apps

In order to use Store Framework and work on your store theme, it is needed to have both `vtex.store-sitemap` and `vtex.store` installed.

Run  `vtex list`  and check whether those apps are already installed.

If they aren't, run the following command to install them: `vtex install vtex.store-sitemap vtex.store -f`

### Step 5 - Uninstalling any existing theme

By running `vtex list`,  you can verify if any theme is installed.

It is common to already have a `vtex.store-theme`  installed when you start the store's front development process.

Therefore, if you find it in the app's list, copy its name and use it together with the command `vtex uninstall`. For example:

```json

vtex uninstall vtex.store-theme
```
### Step 6- Run and preview your store
Then time has come to upload all the changes you made in your local files to the platform. For that, use the vtex link command.

If the process runs without any errors, the following message will be displayed: App linked successfully. 

Then, run the vtex browse command to open a browser window having your linked store in it.

This will enable you to see the applied changes in real time, through the account and workspace in which you are working.

## Dependencies
All store components that you see on this document are open source too. Production ready, you can found those apps in this GitHub organization.
Store framework is the baseline to create any store using VTEX IO Web Framework.
- Store
Store GraphQL is a middleware to access all VTEX APIs.
- Store GraphQL

### Store Component Apps
- Header
- Footer
- Slider Layout
- Shelf
- Telemarketing
- Menu
- Login
- Minicart
- Category Menu
- Product Summary
- Breadcrumb
- Search Result
- Product Details
- Store Components

### Peer store component dependencies
```json
"peerDependencies": {
    "vtex.mega-menu": "2.x",
    "vtex.questions-and-answers": "0.x"
  }
```

### Custom component dependencies

 ```json
 "dependencies": {
    "itgloberspartnercl.whatsapp-button": "0.x",
    "itgloberspartnercl.bullets-diagramation": "0.x",
    "itgloberspartnercl.add-to-cart-info": "0.x",
    "itgloberspartnercl.custom-department-search": "0.x",
    "itgloberspartnercl.pdf-reader": "0.x",
    "itgloberspartnercl.quick-order": "0.x",
    "itgloberspartnercl.special-diagramation": "0.x"
}
```

### Documentation to be considered
- Gitflow
- Code Standard
- Semantic Commit
