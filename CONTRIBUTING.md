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

`"data": {`
`"marketing-page-about-title": "About andcards - who we are and what we do | andcards"`,
`"marketing-page-about-description": "Who is the developer of andcards? Learn about the coworking space marketplace and software.",`
`...`
`}`

- Follow it's position on a page.

Example:

`"suite-page-organization-settings-spaces-section-amenities": "Amenities"`

`"suite-page-organization-settings-spaces-section-amenities-parking": "Parking"`

- Include the component name as part of the key.

Example:

`"suite-page-organization-settings-spaces-section-amenities-button-add": "Add amenities"`

- The alert translations begins with an `alert` word.

Example:

`"alert-confirmation-organization-leave-no": "Cancel"`

## Want to add a new locale?

1. Fork this repository.
2. Create a file with a name of a language code in each folder right next to existing translations. For example, for a Spanish language you need to create a `es.json` file in each folder.
3. Make a Pull Request.

### Recommendations

For making a translation process simpler, we recommend copy and pasting existing translations, for example, English, onto a newly created file and then translate.

## Localization Style Guide

### 1. Avoid redundancies.

If an element appears in a section and it's meaning can be contextually implied, don't repeat the keyword. For example, if a page is "Add Plan", there is no need to repeat the word "plan" on the page.

- "Type plan description" → "Type a description"
- "Type plan name" → "Type a name"

### 2. Reduce clauses to phrases.

- "To change sorting preferences, find a button which is located in Settings." → "Change sorting in Settings."
- "Unfortunately, you have no permission to access." → "No access permission."

### 3. Do not use intensifiers.

- "It is really important to set a secure password." → "Set a secure password."
- "Please enter the booking title." → "Type a title."
- "Please indicate how many of such plans you offer." → "Type a quantity."

### 4. Avoid expletive constructions.

- "There is a setting to change a password in Settings." → "Change a password in Settings."
- "Looks like this workspace name is already taken. Try another one." → "The name is already taken. Try another one."
- "Choose if members must indicate the title when they create bookings." → "Require members to type a title."

### 5. Avoid pronouns.

- "You cannot book for past dates." → "Unable to book in the past."
- "Your trial is ended." → "The trial is over."
- "You don't have a permission to complete the action." → "No permission to complete the action."

In particular, don't use "he," "him," "his," "she," or "her" as gender-neutral pronouns, and don't use "he/she" or "(s)he" or other such punctuational approaches.

More about using pronouns: https://developers.google.com/style/pronouns

### 6. Use only short forms of the modal verbs can, could, shall, should, must, will and would.

- "Last login method cannot be deleted." → "The last login method can't be deleted."
- "Cannot load current session details." → "Can't load current session details."

### 7. Use articles (English and Spanish).

Include `a`, `an`, and `the` in your writing. Use `a` and `an` with singular nouns when in general context. Use `the` with a singular or plural nouns to refer to specific elements that already exist on the page.

- "Dates should match selected criteria." (general context plural nouns don't need an article)
- "The trial is over." (referring to a singular noun, specifically a booking system trial)
- "Type a name." (referring to a singular noun in general context)

More details on articles: https://developers.google.com/style/articles

### 7. Capitalize the first letter of each word in titles (English only).

- "All membership plans" → "All Membership Plans"
- "Link printer account" → "Link Printer Account"

### 8. Capitalize the first letter of each word in buttons (English only).

Use verbs that precisely describe the button’s action. For example, `Cancel`, `Clear History`, `Add Email`, `Select All`, etc.

### 9. Avoid professional jargon and use proper terminology.

| DE   | EN        | ES       | UK           | RU           | KO   |
| ---- | --------- | -------- | ------------ | ------------ | ---- |
| Einstellungen | Settings  | Settings | Налаштування | Настройки    | 설정 |
| Workspace | Workspace | Espacio  | Коворкінг    | Коворкинг    | 공간 |
| Buchung | Booking   | Reserva  | Резервація   | Бронирование | 예약 |
| Raum | Room      | Sala     | Кімната      | Переговорная | 회의실 |

Never use wrong forms: organization (EN), sala de habitacion (ES), бронювання (UK), резервация (RU). In Korean, prefer "-세요" to "-하십시요": "제목을 입력하세요."
