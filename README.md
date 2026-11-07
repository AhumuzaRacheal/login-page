# Online Application Portal (MUST Admissions Interface)

A pixel-perfect, fully interactive recreation of the **Mbarara University of Science & Technology (MUST) Online Application Portal** (`applications.must.ac.ug`), designed based on the portal login and registration screenshots.

---

## 🌟 Key Features

1. **Sign-In View (Image 2)**:
   - **University Header**: University shield branding & "Need Help?" quick link.
   - **Portal Pill Badge**: Clean `"Online Application Portal"` badge with live indicator.
   - **Login Form**:
     - Email address field with mail icon.
     - Password field with padlock icon and **show/hide password toggle** button.
     - **Sign In** action button with authentic icons.
   - **Forgot Password**: Opens a modal to request password reset via registered email/SMS.
   - **How to Apply**: Comprehensive admissions guide modal with step-by-step instructions.

2. **Create Account Modal (Image 1)**:
   - Modal dialog with blurred backdrop overlay and close button.
   - Fields matching the screenshot:
     - **Surname** (with user silhouette icon).
     - **Other Names** (with dual user icon).
     - **Phone Number** with country code selector (`Uganda (+256)` default, Kenya `+254`, Tanzania `+255`, Rwanda `+250`, etc.) and helper guidance text.
     - **Email Address** with direct shortcut link (`Don't have an Email? Click to create ➔`).
   - Action buttons: **Close** and **+ Create Account**.

3. **Interactive Simulation & Applicant Dashboard**:
   - Creating an account automatically generates a realistic temporary password (e.g. `MUST-XXXXXX`) and pops up the confirmation screen with a 1-click **Copy to Clipboard** button.
   - Signs into the **Applicant Dashboard**:
     - Real-time step progress tracker (`Account Created` ➔ `Personal Details` ➔ `Program Selection` ➔ `Documents & Fee`).
     - Study program selector (Medicine & Surgery MBChB, Computer Science BCS, Software Engineering BSE, etc.).
     - Payment Reference Number (PRN) generator for application fee (UGX 50,000 / USD 50).
     - Logout and session persistence via `sessionStorage` & `localStorage`.

---

## 🚀 How to Run the Website

### Option 1: Using the Included Python Server
Open a terminal in this directory and run:

```bash
python3 server.py 8080
```

Then visit [http://localhost:8080](http://localhost:8080) in your web browser.

### Option 2: Direct Browser Opening
Simply double-click or open [index.html](file:///home/ahumuza/.gemini/antigravity/scratch/online-application-portal/index.html) directly in any web browser (Chrome, Edge, Firefox, Safari).

---

## 📁 File Structure

```
online-application-portal/
├── index.html     # Semantic HTML5 layout (Login, Modals, Applicant Dashboard)
├── styles.css     # CSS styling, typography, colors, shadows & responsive rules
├── app.js         # Interactive engine, validation, local storage, toast notifications
├── server.py      # Python 3 local development server
└── README.md      # Documentation and integration guide
```

---

## 🔑 Demo Account Credentials

For quick testing without creating a new account:
- **Email**: `demo@must.ac.ug`
- **Password**: `Password123`

You can also click **"+ Create Account"** to create any applicant with custom details!
