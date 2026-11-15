# Student Loan App

> 👨‍💻 Developed by **[Suresh Kumar Meesala](https://github.com/SureshKumarMeesala)** · 🎨 UI design by **Milton Solis** (credits below)

A mobile app built with **React Native (0.88+)**, **Expo SDK 58+** and **Expo Router**, using **JavaScript and JSX (`.js`, `.jsx`)**. Every screen is built from the original Sketch design `student-loan-app-milton-solis.sketch` by **Milton Solis**: one route per artboard, with the artboard's layout, colours, images and text.

![Student Loan App screens](./showcase.jpg)

## 📱 Screens (31 design artboards)

Listed in the order of the app's flow. "Taps" is the number of tap targets wired on the screen (buttons, tabs, back arrows, list rows).

| # | Screen (artboard) | Route | Size | Taps |
|---|---|---|---|---|
| 1 | **02_welcome_01** · start screen | `src/app/s-02-welcome-01.jsx` | 1125 × 2436 | 3 |
| 2 | **01_login_01** | `src/app/s-01-login-01.jsx` | 1125 × 2436 | 3 |
| 3 | **01_sign_post_01** | `src/app/s-01-sign-post-01.jsx` | 1125 × 2436 | 2 |
| 4 | **02_signUp_01** | `src/app/s-02-signup-01.jsx` | 1125 × 2436 | 2 |
| 5 | **02_welcome_02** | `src/app/s-02-welcome-02.jsx` | 1125 × 2436 | 4 |
| 6 | **02_welcome_03** | `src/app/s-02-welcome-03.jsx` | 1125 × 2436 | 4 |
| 7 | **02_welcome_04** | `src/app/s-02-welcome-04.jsx` | 1125 × 2436 | 4 |
| 8 | **02_welcome_05** | `src/app/s-02-welcome-05.jsx` | 1125 × 2436 | 4 |
| 9 | **04_dashboard_01_b_01** | `src/app/s-04-dashboard-01-b-01.jsx` | 1125 × 2436 | 2 |
| 10 | **04_dashboard_01_b_02** | `src/app/s-04-dashboard-01-b-02.jsx` | 1125 × 2436 | 2 |
| 11 | **04_dashboard_01_c_01** | `src/app/s-04-dashboard-01-c-01.jsx` | 1125 × 2436 | 2 |
| 12 | **04_dashboard_01_c_02** | `src/app/s-04-dashboard-01-c-02.jsx` | 1125 × 2436 | 2 |
| 13 | **05_transactions_list_01** | `src/app/s-05-transactions-list-01.jsx` | 1125 × 2436 | 2 |
| 14 | **05_transactions_list_02** | `src/app/s-05-transactions-list-02.jsx` | 1125 × 2436 | 3 |
| 15 | **06_ch_pool_01_all** | `src/app/s-06-ch-pool-01-all.jsx` | 1125 × 2436 | 6 |
| 16 | **06_ch_pool_02_recurring** | `src/app/s-06-ch-pool-02-recurring.jsx` | 1125 × 2436 | 4 |
| 17 | **06_ch_pool_03_one** | `src/app/s-06-ch-pool-03-one.jsx` | 1125 × 2436 | 5 |
| 18 | **06_ch_pool_04_invite** | `src/app/s-06-ch-pool-04-invite.jsx` | 1125 × 2436 | 2 |
| 19 | **07_savings_01** | `src/app/s-07-savings-01.jsx` | 1125 × 2436 | 2 |
| 20 | **07_savings_02_recurring_b_01** | `src/app/s-07-savings-02-recurring-b-01.jsx` | 1125 × 2436 | 2 |
| 21 | **07_savings_03_roundups** | `src/app/s-07-savings-03-roundups.jsx` | 1125 × 2436 | 2 |
| 22 | **08_settings_01** | `src/app/s-08-settings-01.jsx` | 1125 × 2436 | 2 |
| 23 | **08_settings_02_details** | `src/app/s-08-settings-02-details.jsx` | 1125 × 2436 | 2 |
| 24 | **08_settings_03_banks** | `src/app/s-08-settings-03-banks.jsx` | 1125 × 2436 | 4 |
| 25 | **08_settings_03_banks_b** | `src/app/s-08-settings-03-banks-b.jsx` | 1125 × 2436 | 2 |
| 26 | **08_settings_04_loans** | `src/app/s-08-settings-04-loans.jsx` | 1125 × 2436 | 2 |
| 27 | **08_settings_04_loans_b** | `src/app/s-08-settings-04-loans-b.jsx` | 1125 × 2436 | 2 |
| 28 | **10_link_bank_01** | `src/app/s-10-link-bank-01.jsx` | 1125 × 2436 | 2 |
| 29 | **10_link_bank_02** | `src/app/s-10-link-bank-02.jsx` | 1125 × 2436 | 2 |
| 30 | **10_link_bank_03** | `src/app/s-10-link-bank-03.jsx` | 1125 × 2436 | 3 |
| 31 | **10_link_bank_04** | `src/app/s-10-link-bank-04.jsx` | 1125 × 2436 | 2 |

Screenshots of every screen are in [`screenshots/`](./screenshots).

## 🧩 How it's built

- `src/screens/*.json`: each design artboard converted to screen data (vector shapes, gradients, image fills, masks, shadows, blurs and rich text, positioned as in the design), plus its tap targets
- `src/sketch/SketchScreen.jsx`: draws a screen at the device's width with `react-native-svg`, native `Text`/`TextInput` and `expo-blur`, and handles navigation between screens
- `src/app/`: Expo Router routes, one per artboard (`index.jsx` opens the start screen)
- `assets/images/`: images used by the design

## 🛠️ Tech Stack

- **Framework**: React Native 0.88+ / Expo SDK 58+
- **Navigation**: Expo Router (file-based routing)
- **Language**: JavaScript & JSX (`.js`, `.jsx`)
- **Rendering**: `react-native-svg`, `expo-blur`
- **Fonts**: Google Fonts via `@expo-google-fonts` (Poppins), standing in for the design's original fonts where those aren't free

<!-- run-locally:start -->

## ▶️ Run locally

```bash
npm install
npx expo start
```

Then press `i` for the iOS simulator, `a` for Android, or `w` for the web, or scan the QR code with Expo Go.

<!-- run-locally:end -->

<!-- developer:start -->

## 👨‍💻 Developer

This React Native app was developed by **Suresh Kumar Meesala**.

| | |
|---|---|
| Developer | [Suresh Kumar Meesala](https://github.com/SureshKumarMeesala) |
| GitHub | [@SureshKumarMeesala](https://github.com/SureshKumarMeesala) |
| Organization | [FreeAppSource](https://github.com/FreeAppSource) |
| Repository | <https://github.com/FreeAppSource/student-loan-app> |

<!-- developer:end -->

---

<!-- design-credits:start -->

## 🎨 Design Credits

This app is based on the free **Student Loan App** design by **Milton Solis**, downloaded from Sketch App Sources. All visual design credit goes to the designer. The screens are reproduced from the original Sketch file; fonts that aren't free are replaced with similar Google Fonts, so some details may differ slightly from the original.

| | |
|---|---|
| Designer | [Milton Solis](https://www.sketchappsources.com/contributor/miltonsolis) |
| Original design | [Student Loan App](https://dribbble.com/shots/6934968-Chipper-Student-Loan-App-case-study-Free-UI-kit) |
| Downloaded from | [Sketch App Sources](https://www.sketchappsources.com/free-source/4086-student-loan-app-sketch-freebie-resource.html) |
| Dribbble | <http://www.dribbble.com/milton_solis> |
| Website | <https://www.behance.net/milton_solis> |
| Original file | `student-loan-app-milton-solis.sketch` |
| License / usage | Not stated on the page. Free download; give credit (Sketch App Sources Terms). Confirm with the designer before commercial use. |

**Attribution:**

> UI design: "Student Loan App" by Milton Solis (https://dribbble.com/shots/6934968-Chipper-Student-Loan-App-case-study-Free-UI-kit), downloaded from Sketch App Sources (https://www.sketchappsources.com/free-source/4086-student-loan-app-sketch-freebie-resource.html).

The original design source files are not included in this repository; get them from the links above. This app's **code** is released under the [MIT License](./LICENSE); the visual design remains the designer's (see [NOTICE](./NOTICE)).

Photos, brand logos and avatars inside the design may belong to third parties and are not covered by the designer's permission.

<!-- design-credits:end -->
