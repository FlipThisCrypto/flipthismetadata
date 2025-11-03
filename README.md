# FlipThisMetadata 🏷️

A powerful, single-file HTML/JavaScript tool designed to generate compliant metadata for Chia (XCH) NFTs, supporting both the standard **CHIP-0007** and the enhanced **CHIP-0015** Data Layer standard.

Built with **Tailwind CSS** for a clean, modern, and responsive user experience.

---

## ✨ Features

* **Dual Standard Support:** Automatically defaults to **CHIP-0007**. If the Data section is filled, the generator intelligently switches the output `format` to **CHIP-0015**.
* **Dynamic Data Section:** Includes a **toggle** to show/hide the complex CHIP-0015 fields (Data URL, Thumbnail, Creator, etc.), keeping the interface clean for simpler metadata creation.
* **Intuitive Interface:** Easily add and remove **Top-Level Attributes** (Traits) and **Collection Attributes**.
* **Real-time JSON Output:** See the metadata update instantly as you type, ensuring compliance before you mint.
* **Clean Output:** Empty fields, including entire nested objects like `data` or `collection`, are automatically omitted from the final JSON for a clean, minimal file structure.

---

## 🚀 How to Use

This project is a single, self-contained `index.html` file. No server or build process is required!

1.  **Clone or Download:** Get the `index.html` file from this repository.
2.  **Open in Browser:** Double-click the `index.html` file to open it in any modern web browser (Chrome, Firefox, Edge, etc.).
3.  **Fill the Form:** Enter your core NFT information (Name, Description, Collection details, Attributes).
4.  **Enable CHIP-0015 (Optional):** Check the **"Enable CHIP-0015 (Data) Fields"** box to access the detailed Data, Thumbnail, and Creator sections required for advanced data standards.
5.  **Copy Metadata:** Once the JSON output is complete on the right panel, click **"Copy to Clipboard"** and paste the result into your NFT minting tool.

---

## 💻 Project Structure

The entire application is contained within one file, making it perfect for rapid deployment or local usage.

| File | Description |
| :--- | :--- |
| `index.html` | The single-file application. Contains all HTML structure, **Tailwind CSS** framework links, and the core **JavaScript** logic. |

---

## 🛠️ Technology Stack

* **HTML5:** Structure
* **JavaScript:** Core application logic, form handling, and JSON generation.
* **Tailwind CSS (CDN):** Styling and responsive design.

---

## 💡 Customization & Contribution

Feel free to fork this project and customize it for different collections or metadata standards!

1.  **Add Attributes:** To add more default `trait_type` or `value` attributes, modify the `addAttributeRow` function calls in the JavaScript.
2.  **Modify Data Types:** The dropdown lists for `@type` values (e.g., `DigitalDocument`, `Person`) can be easily updated within the HTML `<select>` elements.
3.  **Enhance Logic:** The core logic for standard switching is within the `generateJson()` function, allowing for easy updates to new CHIP standards as they emerge.
