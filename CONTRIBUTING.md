## Naming principles

### Folders

- Follow the component name.
- Words are lower-cased and separated with dashes.

Example:

- Component name: `PageOrganizationCompanyProfile`.
- Folder with translations name: `page-organization-company-profile`.

### Translation keys

- Sorted in alphabetical order.

- Titles and descriptions should be on the top of the file.

Example: 

`"marketing-page-about-title": "About andCards - who we are and what we do | andCards"`,
`"marketing-page-about-description": "Who is the developer of andCards? Learn about the coworking space marketplace and software.",`
...

- Follow it's position on a page.

Example: 

`"suite-page-organization-company-profile-section-amenities": "Amenities"`

`"suite-page-organization-company-profile-section-amenities-parking": "Parking"`

- Include the component name as part of the key.

Example:

`"suite-page-organization-company-profile-section-amenities-button-add": "Add amenities"`

- The alert translations begins with an `alert` word. 

Example:

`"alert-confirmation-organization-leave-no": "Cancel"`

## Want to add a new locale?

1. Fork this repository.
2. Create a file with a name of a language code in each folder right next to existing translations. For example, for a Spanish language you need to create a `es.json` file in each folder.
3. Make a Pull Request.

### Recommendations

For making a translation process simpler, we recommend copy and pasting existing translations, for example, English, onto a newly created file and then translate.
