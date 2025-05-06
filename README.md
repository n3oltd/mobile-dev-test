## Coding Task (React / Capacitor)

This coding task is for a mobile developer and assumes that you are familiar with React and Capacitor.

Your task is to build a simple UI which consumes the provided API and demonstrates the below functionality.

There is no absolute time limit and we won't judge you on how long it took you to complete, however we would suggest you spend no more than 4 hours on this task. We wouldn't ask you to do this task if we didn't already think you looked like a good candidate, so we really appreciate the time you put into this.

### General Instructions

- Please use recent version of **React** and **Capacitor**
- Use Ionic.
- Use TypeScript.
- You are not required to use a state management library but may if you wish.
- Use any toolchain you wish, but make sure you provide a **README** so we know how to run your app.

### The Task

Please build a simple cross platform mobile application which allows the user to view donation items and create new donation items. Further details about what this means can be found below. At the very minimum your mobile application should show a splash/welcome screen for 3 seconds, display a login prompt (you can hardcode any username/password for now), and a main screen for managing donation items.

A donation item is an item which can be donated towards by a donor, similar to a product in an e-commerce setting.

Using Ionic, please build a simple UI which integrates with the API provided. The user should be able to:

- View a list of the current donation items. Please show:
  - Donation item Name
  - Reference (e.g. DI1001)
  - Price
  - Status
  - Location
  - Theme
- Filter the donation items by their Status
- Add a new donation item

To create a donation item, pass the following properties:

| Property | Description                                                   | Validation                                                                                   | Required on Create Request |
| -------- | ------------------------------------------------------------- | -------------------------------------------------------------------------------------------- | -------------------------- |
| Name     | A descriptive name of the donation item                       | - Length between 1-200 <br> - Must be unique                                                 | Yes                        |
| Location | The id of the location where this donation will be spent      | - Must be valid location                                                                     | Yes                        |
| Theme    | The id of the theme towards which this donation will be spent | - Must be valid theme                                                                        | Yes                        |
| Price    | The suggested amount in GBP (£) for this donation item        | - Must be a number/decimal if provided <br> - Currency must be GBP <br> - Amount must be > 0 | No                         |

### The API

All API endpoints are accessible and documented at:

https://n3o-coding-task-react.azurewebsites.net/swagger/index.html

You can use the /reset endpoint to reset the in-memory database.

### Submitting

Please share your solution as a zip file with a working apk so we can test your solution on Android.

We look forward to seeing your work!

If you have any questions or any of the requirements are unclear please feel free to get in touch.
