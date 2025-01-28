# Care Connect

Care Connect is an innovative healthcare project designed to streamline communication between patients and nurses. The platform enables patients to record their voice messages detailing their health concerns. These messages are prioritized and sent to the nurse, who can address the issues efficiently. The project is divided into the following components:

1. **AI Part**: This component processes patient voice recordings using advanced algorithms. It analyzes the content to identify the patient's concerns, assigns a priority level based on the urgency, and makes the data available for the backend.

2. **Backend**: The backend acts as the central processing hub for the system. It handles:
   - Storing patient data and voice recordings.
   - Communicating with the AI component to retrieve analysis results.
   - Managing user authentication and authorization.
   - Sending processed data to the frontend interfaces for display. (Implemented in Node.js)

3. **Frontend**: The frontend is the user interface layer, offering distinct functionalities for three types of users:
   - **Admin**: The admin dashboard allows management of user accounts, monitoring of system performance, and review of overall operations.
   - **Nurse**: The nurse dashboard displays patient concerns prioritized by the AI component, enabling nurses to address the most critical cases first.
   - **Patient**: The patient interface provides a simple way to record and submit voice messages detailing health issues.

---

## Features

- **Seamless Communication**: Patients can easily record and send voice messages.
- **AI-Driven Prioritization**: Automatically prioritizes patient concerns based on urgency.
- **User-Specific Dashboards**: Customized interfaces for admins, nurses, and patients.
- **Scalable Architecture**: Modular design to facilitate future enhancements.

---

## How to Set Up the Project

Follow the steps below to set up and run each component of Care Connect:

### 1. AI Component

The AI component processes patient voice inputs. Here’s how to set it up:

#### Steps:

1. **Navigate to the AI Directory:**
   ```bash
   cd AI-part
   ```

2. **Create a Python Virtual Environment:**
   ```bash
   python -m venv env
   source env/bin/activate  # For Linux/Mac
   env\Scripts\activate   # For Windows
   ```

3. **Install Required Libraries:**
   ```bash
   pip install -r requirements.txt
   ```

4. **Run the AI Component:**
   ```bash
   uvicorn app:app --reload
   ```

### 2. Backend

The backend manages data flow and interactions between the AI and frontend. It is implemented in Node.js.

#### Steps:

1. **Navigate to the Backend Directory:**
   ```bash
   cd backend-careconnect
   ```

2. **Install Dependencies:**
   ```bash
   npm install
   ```

3. **Run the Backend Server:**
   ```bash
   npm start
   ```

### 3. Frontend for admin

The frontend provides the user interfaces for admin roles.

#### Steps:

1. **Navigate to the Frontend Directory:**
   ```bash
   cd SpringBoardApp_Admin_App
   ```

2. **Install Frontend Dependencies:**
   If using a framework like React or Angular:
   ```bash
   npm install
   ```

3. **Run the Frontend Application:**
   ```bash
   npm start
   ```

### 4. Frontend for nurse, patient

The frontend provides the user interfaces for nurse, and patient roles.

#### Steps:

1. **Navigate to the Frontend Directory:**
   ```bash
   cd SpringBoardApp_FrontEnd
   ```

2. **Install Frontend Dependencies:**
   If using a framework like React or Angular:
   ```bash
   npm install
   ```

3. **Run the Frontend Application:**
   ```bash
   npm start
   ```

### 5. Running the Entire System

Run each component in separate terminals:

- **Terminal 1**: Run the AI Component as described in the AI setup.
- **Terminal 2**: Run the Backend as described in the backend setup.
- **Terminal 3**: Run the Frontend as described in the frontend setup.

Once all components are running, you can interact with the system through the frontend interfaces.

---

## Folder Structure

```
care_connect/
|-- aipart/            # AI processing
            |-- requirements.txt 
|-- backend-careconnect/           # Backend APIs (Node.js)
|-- SpringBoardApp_Admin_App/      # Frontend interface for admin
-- SpringBoardApp_FrontEnd/        # Frontend interface for nurse,patient
```

---

## Notes

- Ensure all required dependencies are installed.
- Use the latest version of Python and Node.js for compatibility.
- For any issues, refer to the documentation or contact the development team.

---

## Contribution
We welcome contributions to improve Care Connect. Feel free to open issues or submit pull requests on the project repository.

---

## License

This project is licensed under the MIT License. See the LICENSE file for details.
