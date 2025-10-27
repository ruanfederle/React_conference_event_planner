# coding-project-template


🏢 Conference Expense Planner

The **Conference Expense Planner** is a React + Redux-based application that helps users plan, calculate, and visualize the total cost of hosting a conference or event.
It allows users to choose **venues**, **add-ons (A/V equipment)**, and **meals**, and automatically computes subtotals and overall expenses.

---

🚀 Features

🏛️ **Venue Selection** – Choose from multiple event rooms with capacity limits.
🎧 **Add-ons Management** – Add or remove audiovisual (A/V) items like projectors and microphones.
🍽️ **Meal Planning** – Select meal options and specify the number of attendees.
💰 **Dynamic Cost Calculation** – Automatically calculates subtotal and total costs per category.
🔁 **Redux-Powered State Management** – Uses `useSelector` and `useDispatch` for centralized and predictable state handling.
🧾 **Detailed Summary View** – Toggle between item selection and a detailed total cost breakdown.

---

🧩 Tech Stack

| Technology           | Purpose                                    |
| -------------------- | ------------------------------------------ |
| **React**            | Frontend UI library                        |
| **Redux Toolkit**    | State management for venue, A/V, and meals |
| **CSS**              | Styling and layout                         |
| **JavaScript (ES6)** | Application logic                          |

---

⚙️ Installation & Setup

### 1. Clone the repository

```bash
git clone https://github.com/ruanfederle/conference-expense-planner.git
```

### 2. Navigate to the project folder

```bash
cd conference-expense-planner
```

### 3. Install dependencies

```bash
npm install
```

### 4. Start the development server

```bash
npm start
```

### 5. Open in your browser

Visit: [http://localhost:3000](http://localhost:3000)

---

🧠 How It Works

1. **Venues:**

   * Users can select different halls or rooms.
   * The "Auditorium Hall" has a **maximum capacity of 3** (hard-coded limit).

2. **Add-ons:**

   * Users can increment or decrement the number of A/V equipment items (like projectors or microphones).

3. **Meals:**

   * Users specify the **number of attendees** and select meal options.
   * The total meal cost scales with the number of people.

4. **Cost Summary:**

   * Clicking **“Show Details”** displays all selected items with subtotals.
   * Uses `TotalCost` component for displaying the breakdown.

---

🧮 State Management (Redux)

Each category (venue, add-ons, meals) is managed in its own Redux slice:

* `venueSlice.js` → Handles venue selection and quantity limits.
* `avSlice.js` → Manages audiovisual items.
* `mealsSlice.js` → Handles meal selection and attendee count.

---

🎨 Styling

All UI styling is handled in:

```
ConferenceEvent.css
```

You can customize the appearance by editing button classes, table layouts, or color themes.

---

🧱 Components Overview

| Component                                   | Description                                                    |
| ------------------------------------------- | -------------------------------------------------------------- |
| **ConferenceEvent**                         | Main component handling event planning logic and UI rendering. |
| **TotalCost**                               | Displays total cost summary with subtotals per section.        |
| **venueSlice**, **avSlice**, **mealsSlice** | Redux slices managing application state.                       |

---

🧰 Example Usage

```bash
# User flow:
1. Choose a venue (max 3 for Auditorium).
2. Add projectors or microphones.
3. Specify number of attendees and select meal options.
4. Click "Show Details" to view the total expense breakdown.
```

---

📸 Screenshots (Optional)

* Venue selection view
<img width="1675" height="956" alt="image" src="https://github.com/user-attachments/assets/c854cacc-19b4-4f07-b870-9eaa8822dc54" />

* Detailed summary page
<img width="1670" height="954" alt="image" src="https://github.com/user-attachments/assets/294d2720-d78f-40ba-a078-72bdb7431738" />


---

📜 License

This project is licensed under the **MIT License** – feel free to use, modify, and distribute it.

---

## 👨‍💻 Author

**Ruan Federle**
📧 [[ruanfederle@hotmail.com](mailto:ruanfederle@hotmail.com)]
🔗 [GitHub Profile](https://github.com/ruanfederle)

---

