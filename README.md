# Innovator Welcome Page

This community project adds a new form to greet the user when first logging into Innovator. It uses a method called `aras.MetadataCache.GetConfigurableUiAsync` to grab the cached TOC, and then restructures it into the Homepage. Administrators can set the welcome_page form as a "Start Page" for individual Users. 

The startpage allows users to quickly launch searches for any ItemType they have access to. It also allows them to easily create a new Item, as long as they have the correct permissions to do so. 

The welcome page is also included in the TOC. The TOC Access of the welcome_page ItemType is set to world, because TOC Access is necessary for a designated Start Page. This also allows users to get back to the welcome screen at any point. 
 

Release | Notes
--------|--------
[v1.0](https://github.com/ArasLabs/innovator-welcome-page/releases/tag/v1.0) | First release of the Innovator Welcome Page project
#### Supported Aras Versions

Project | Aras
--------|------
[v1.0](https://github.com/ArasLabs/innovator-welcome-page/releases/tag/v1.0) | 12.0 SP0, SP1

## Installation

#### Important!
**Always back up your code tree and database before applying an import package or code tree patch!**

### Pre-requisites

1. Aras Innovator installed
2. Aras Package Import tool
3. **innovator-welcome-page** import packages

### Install Steps

1. Backup your database and store the BAK file in a safe place.
2. Open up the Aras Package Import tool.
3. Enter your login credentials and click **Login**
  * _Note: You must login as root for the package import to succeed!_
4. Point the import tool to the `imports.mf` file within the repository
5. Select Merge/Thorough
   

## Usage

1. As an Administrator, select the designated user
2. Set the user's starting page property to "Welcome Page"
3. Log in as a user with the updated Start Page.
4. Click an item to launch a search, and click the new button to create a new version of that Item. 

## Contributing

1. Fork it!
2. Create your feature branch: `git checkout -b my-new-feature`
3. Commit your changes: `git commit -am 'Add some feature'`
4. Push to the branch: `git push origin my-new-feature`
5. Submit a pull request

For more information on contributing to this project, another Aras Labs project, or any Aras Community project, shoot us an email at araslabs@aras.com.

## Credits

Created by AJ Sebastian, Aras Labs.

## License

Aras Labs projects are published to Github under the MIT license. See the [LICENSE file](./LICENSE.md) for license rights and limitations.
