FlipThisMetadata
FlipThisMetadata is a lightweight, browser-based tool designed to generate compliant JSON metadata for Chia Network NFTs.

It streamlines the creation of metadata files by providing a user-friendly interface for inputting data, automatically formatting it to CHIP-0007 standards, and optionally extending it with CHIP-0015 off-chain data fields.

🚀 Features
Standard Compliance: formatting for CHIP-0007 (NFT Metadata) and CHIP-0015 (Off-chain Data).

Zero Dependencies: Built with vanilla JavaScript and Tailwind CSS (via CDN). No npm install or build steps required.

Local SHA256 Hashing: Includes a Drag-and-Drop tool to calculate file hashes directly in the browser. Your files never leave your computer.

Collection Management: Built-in UUID v4 generator for Collection IDs.

Dynamic Attributes: Easily add, remove, and manage trait attributes and collection attributes.

Live Preview: Real-time JSON syntax highlighting as you type.

Smart Auto-fill: Automatically detects encoding formats based on selected file types (e.g., selecting DigitalDocument sets format to application/pdf).

🛠 Standards Supported
CHIP-0007: The core standard for defining NFT names, descriptions, attributes (traits), and collection information.

CHIP-0015: An extension for linking rich off-chain data (PDFs, Videos, 3D Models) with hash verification (sha256), encoding formats, and creator attribution.

📦 Installation & Usage
Since this is a client-side tool, there is no backend to configure.

Option 1: Run Locally (Recommended)
Clone the repository:

Bash

git clone https://github.com/your-username/flip-this-metadata.git
Navigate to the folder:

Bash

cd flip-this-metadata
Open index.html in any modern web browser.

Option 2: Hosted
Because this is a static file, you can host it immediately using GitHub Pages, Vercel, or Netlify by simply pointing them to this repository.

📖 How to Use
1. Core Info
Fill in the basic details of your NFT (Name, Description, Minting Tool).

2. Attributes
Click "Add Top-Level Attribute" to define traits (e.g., Background: Blue, Rarity: Legendary).

3. Collection Data
Enter your Collection Name.

Click Generate UUID to create a unique Collection ID (v4 Standard).

Add specific collection attributes if necessary.

4. CHIP-0015 Data (Optional)
Toggle "Enable CHIP-0015 Data Fields" to access advanced options:

SHA256 Tool: Drag your asset (image, PDF, video) onto the drop zone. The tool will calculate the hash and automatically fill the sha256 field for you.

Creator Info: Add attribution for the organization or person behind the NFT.

Thumbnails: Define separate thumbnail assets with their own hashes and URLs.

5. Export
Once finished, click Copy to Clipboard to grab the raw JSON, or hit Reset to start over.

🔒 Privacy & Security
Client-Side Only: All logic runs inside your browser.

No Data Collection: No data is sent to any external server.

Local Hashing: The SHA256 calculator uses the browser's SubtleCrypto API. Your files are processed in memory and are not uploaded anywhere.

💻 Tech Stack
HTML5

JavaScript (ES6+)

Tailwind CSS (Styling)

Inter Font (Typography)

🤝 Contributing
Contributions are welcome! If you find a bug or want to add a feature (like support for CHIP-0026), please feel free to open an issue or submit a pull request.

Fork the Project

Create your Feature Branch (git checkout -b feature/AmazingFeature)

Commit your Changes (git commit -m 'Add some AmazingFeature')

Push to the Branch (git push origin feature/AmazingFeature)

Open a Pull Request

📄 License
Distributed under the MIT License. See LICENSE for more information.

Made for the Chia Ecosystem.
