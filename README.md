# Stark LaBs - 3D Print Cost Calculator ⚛️

![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)
![Version](https://img.shields.io/badge/version-1.1.0-blue.svg)
![Status](https://img.shields.io/badge/status-active-success.svg)

An advanced, user-friendly web application designed to accurately calculate the cost of 3D printing projects. Built for hobbyists and professionals, this tool goes beyond simple material costs to provide a comprehensive and transparent pricing breakdown.

![Stark LaBs Calculator Screenshot](https://i.imgur.com/YOUR_SCREENSHOT_URL.png) 
*Note: Replace the link above with a URL to a screenshot of your application.*

---

## ✨ Key Features

* **Comprehensive Cost Calculation:** Accurately calculates costs based on materials, electricity, labor, and print failure rates.
* **Advanced Metrics:** Includes fields for often-overlooked costs like machine depreciation, shipping, and design fees.
* **Interactive UI:** A sleek, modern, and fully responsive interface that works seamlessly on desktop, tablets, and mobile devices.
* **Real-time Updates:** All calculations are performed instantly as you input data, providing immediate feedback.
* **Profit Margin Slider:** Easily adjust your profit margin to see the final price for your customers.
* **AI-Powered Features (via Gemini API):**
    * **Marketing Description Generator:** Automatically creates a catchy marketing description for your 3D printed product.
    * **Print Improvement Suggester:** Provides AI-driven tips to enhance print quality and reduce costs.
* **Single-File Application:** The entire application is contained within a single, portable HTML file, requiring no complex setup or dependencies.

---

## 🛠️ Technology Stack

* **Frontend:** HTML5
* **Styling:** [Tailwind CSS](https://tailwindcss.com/)
* **Logic:** Vanilla JavaScript (ES6)
* **AI Integration:** [Google Gemini API](https://ai.google.dev/)

---

## 🧮 How It Works: The Calculation Logic

The calculator is built on a professional methodology that ensures all costs, both direct and indirect, are accounted for.

1.  **Material Cost:** Calculated based on the model's weight relative to the total weight and price of the filament spool.
    ```
    Material Cost = (Model Weight / Spool Weight) * Spool Price
    ```
2.  **Electricity Cost:** Determined by the printer's power consumption, print duration, and the local price per kWh.
    ```
    kWh Used = (Power Consumption (W) * Print Hours) / 1000
    Electricity Cost = kWh Used * Price per kWh
    ```
3.  **Labor Cost:** Quantifies the value of manual work (preparation, post-processing).
    ```
    Labor Cost = Labor Hours * Hourly Rate
    ```
4.  **Failed Print Buffer:** A crucial buffer that adds a percentage of the primary costs to account for potential print failures.
    ```
    Failure Cost = (Material + Electricity + Labor) * (Failure Rate / 100)
    ```
5.  **Total Cost & Final Price:** All costs are summed up, and the desired profit margin is applied to determine the final price for the customer. Additional fees (shipping, design) are then added to get the grand total.
    ```
    Total Cost = (Material + Electricity + Labor + Failure Cost)
    Final Price = Total Cost * (1 + (Profit Margin / 100))
    Grand Total = Final Price + Shipping + Design Fees + Maintenance
    ```

---

## 🚀 Getting Started

No complex installation is required! Because this is a self-contained HTML file, you can run it directly in your web browser.

### Prerequisites

* A modern web browser (e.g., Chrome, Firefox, Edge).
* An internet connection (for the Gemini API features to work).

### Running the Application

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/Ahm3d0x/Stark-LaBs-Calc](https://github.com/Ahm3d0x/Stark-LaBs-Calc)
    ```
2.  **Navigate to the directory:**
    ```bash
    cd [https://github.com/Ahm3d0x/Stark-LaBs-Calc]
    ```
3.  **Open the file:**
    Simply open the `index.html` file in your web browser. You can do this by double-clicking the file or right-clicking and selecting "Open with...".


## 🤝 Contributing

Contributions are what make the open-source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".

1.  Fork the Project
2.  Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3.  Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4.  Push to the Branch (`git push origin feature/AmazingFeature`)
5.  Open a Pull Request

---

## 📜 License

Distributed under the MIT License. See `LICENSE.txt` for more information.

---

## 📧 Contact

Your Name - [Stark LaBs](3d.stark.labs@gmail.com) 

Project Link: [https://github.com/Ahm3d0x/Stark-LaBs-Calc](https://github.com/Ahm3d0x/Stark-LaBs-Calc)
