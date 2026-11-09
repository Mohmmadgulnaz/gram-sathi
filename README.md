# 🌾 Gram Saarathi (ग्राम सारथी)
### Revenue & Crop Disaster Relief Field Workflow Portal

An end-to-end, Hindi-first digital decision-support and workflow management platform for rural revenue officers (लेखपाल / पटवारी / तहसीलदार) to streamline crop disaster assessment, farmer claim verification, and compensation processing.

---

## 📌 1. Problem Statement

During natural disasters such as hailstorms, excessive rainfall, floods, and droughts, farmers submit crop damage compensation claims through manual paperwork.

This creates several challenges:

- **Manual Documentation:** Paper-based claim processing causes delays.
- **Name Mismatches:** Differences between Aadhaar and land records create verification issues.
- **Duplicate Claims:** Joint land ownership can lead to duplicate or incorrect compensation claims.
- **Manual Crop Inspection:** Officers must physically inspect damaged fields and calculate crop loss.
- **Lack of Transparency:** Farmers cannot easily track their application status.

Gram Saarathi aims to digitize and simplify this entire process.

## 🎯 2. Objectives

- Digitize farmer crop damage claims.
- Automate farmer and land-record verification.
- Identify duplicate applications and joint ownership conflicts.
- Calculate affected acreage and estimated compensation.
- Generate digital inspection reports (पंचनामा).
- Provide transparent application tracking.
- Enable human-in-the-loop approval by authorized officers.

## 🚀 3. Key Features

1. **Farmer Registration:** Capture farmer details, land information, and crop details.
2. **Claim Submission:** Submit crop damage claims with supporting documents and photographs.
3. **Land Record Verification:** Compare claimant details against available land records.
4. **Name Matching:** Identify spelling variations and potential identity mismatches.
5. **Duplicate Detection:** Flag duplicate claims and joint land ownership conflicts.
6. **Crop Loss Assessment:** Calculate affected acreage and percentage of crop damage.
7. **33% Damage Threshold:** Flag claims meeting the applicable disaster-relief eligibility threshold for officer review.
8. **Digital Panchanama:** Generate inspection reports with field observations and witness details.
9. **Officer Dashboard:** Track pending, verified, rejected, and approved claims.
10. **Role-Based Access:** Separate workflows for Lekhpal, Revenue Inspector, Naib Tehsildar, and Tehsildar.
11. **Hindi Interface:** Provide a localized interface for rural administrative users.

## 🔄 4. End-to-End Workflow

### Step 1: Farmer Registration & Claim Submission

- Register farmer information.
- Enter Aadhaar-related identification details where legally authorized.
- Enter Khata and Khasra information.
- Select crop type and cultivated area.
- Upload land documents and crop damage photographs.
- Submit the compensation claim.

**Output:** Unique Claim ID and application acknowledgement.

### Step 2: Automated Verification & Field Inspection

- Verify farmer information against available land records.
- Detect possible name mismatches.
- Check joint ownership and individual land shares.
- Identify duplicate applications.
- Assign the claim to the concerned Lekhpal.
- Conduct physical field inspection.
- Record damaged crop area and estimated loss.
- Generate a digital Panchanama.

**Output:** Verified claim with inspection report and flagged discrepancies.

### Step 3: Approval & Compensation Processing

- Lekhpal submits the inspection report.
- Revenue Inspector reviews the claim.
- Naib Tehsildar verifies the supporting documents.
- Tehsildar makes the final administrative decision.
- Calculate eligible compensation according to applicable government guidelines.
- Update the claim status.
- Generate the final approval or rejection report.

**Output:** Approved or rejected claim with a transparent decision record.

## 🔁 5. Application Workflow

```text
Farmer Registration
        |
        v
Crop Damage Claim Submission
        |
        v
Document & Land Record Verification
        |
        v
Duplicate / Name Mismatch Detection
        |
        v
Lekhpal Field Inspection
        |
        v
Crop Loss Assessment
        |
        v
Digital Panchanama Generation
        |
        v
Revenue Inspector Review
        |
        v
Naib Tehsildar Verification
        |
        v
Tehsildar Final Approval
        |
        v
Compensation Processing
        |
        v
Farmer Status Notification
```

## 🛠️ 6. Technology Stack

Update this section according to the technologies actually used in your implementation.

- **Frontend:** React.js
- **Backend:** Node.js / Express.js
- **Database:** MongoDB
- **Programming Language:** JavaScript / Python
- **AI/ML:** Name matching, duplicate detection, and decision-support algorithms
- **Localization:** Hindi language support
- **Version Control:** Git and GitHub

## ⚙️ 7. Installation & Setup

### Step 1: Clone the Repository

```bash
git clone https://github.com/YOUR_USERNAME/gram-saarathi.git
```

### Step 2: Navigate to the Project

```bash
cd gram-saarathi
```

### Step 3: Install Dependencies

For a Node.js project:

```bash
npm install
```

### Step 4: Configure Environment Variables

Create a `.env` file in the project root and configure the required variables.

Example:

```env
PORT=5000
MONGODB_URI=your_mongodb_connection_string
JWT_SECRET=your_secret_key
```

Never commit real passwords, API keys, or secret credentials.

### Step 5: Start the Application

For development:

```bash
npm run dev
```

For production:

```bash
npm start
```

*Note: These commands are illustrative for a Node.js project. Update them according to your actual project structure and package.json scripts.*

## 📂 8. Suggested Project Structure

```text
gram-saarathi/
│
├── frontend/
│   ├── src/
│   ├── components/
│   ├── pages/
│   └── assets/
│
├── backend/
│   ├── controllers/
│   ├── routes/
│   ├── models/
│   ├── middleware/
│   └── server.js
│
├── ml-services/
│   ├── name_matching/
│   ├── duplicate_detection/
│   └── crop_loss_assessment/
│
├── docs/
│   └── workflow.md
│
├── .env.example
├── .gitignore
└── README.md
```

## 🔐 9. Human-in-the-Loop Decision Making

Gram Saarathi is designed as a decision-support system, not an autonomous compensation approval system.

- Automated verification identifies potential errors.
- AI-generated matches are treated as suggestions.
- Officers review discrepancies and supporting documents.
- Physical inspection findings are recorded.
- Final approval and rejection remain with authorized government officials.

## 🌍 10. Expected Impact

- Reduced paperwork and administrative delays.
- Faster crop damage claim verification.
- Improved transparency in compensation processing.
- Better detection of duplicate and incorrect claims.
- Improved accessibility through Hindi localization.
- More efficient coordination between revenue officers.

## 🚧 11. Future Enhancements

- GPS-based field inspection.
- AI-powered crop damage image analysis.
- Offline-first mobile application for field officers.
- SMS/WhatsApp claim status notifications.
- Integration with authorized land-record databases.
- Digital signatures and audit logs.

## 👨‍💻 12. Contribution

Contributions, suggestions, and improvements are welcome.

1. Fork the repository.
2. Create a feature branch.
3. Commit your changes.
4. Submit a Pull Request.

```bash
git checkout -b feature/your-feature
git add .
git commit -m "Add: your feature description"
git push origin feature/your-feature
```

---

**Gram Saarathi – डिजिटल प्रशासन, पारदर्शी सहायता, सशक्त किसान।**

*Empowering farmers through transparent and efficient digital governance.*
