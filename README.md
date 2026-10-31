@import url('https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700&display=swap');

/* 1. Global Variables */

:root {
    --primary: #6477d9;
    --primary-dark: #4e60bf;
    --primary-light: #eef0ff;

    --background: #f7f8fc;
    --surface: #ffffff;

    --text-primary: #252b3b;
    --text-secondary: #7c8499;

    --border: #e9ebf2;

    --success: #39866b;
    --success-bg: #e7f5ee;

    --warning: #b78335;
    --warning-bg: #fff4df;

    --danger: #c85c65;
    --danger-bg: #fdebed;

    --info: #527bc1;
    --info-bg: #eaf1ff;

    --sidebar-width: 250px;

    --radius-sm: 8px;
    --radius-md: 12px;
    --radius-lg: 18px;

    --shadow: 0 4px 20px rgba(35, 45, 80, 0.04);
}

/* 2. Reset */

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

html {
    scroll-behavior: smooth;
}

body {
    font-family: 'Inter', sans-serif;
    background: var(--background);
    color: var(--text-primary);
    font-size: 14px;
    line-height: 1.6;
}

button,
input,
select,
textarea {
    font: inherit;
}

button {
    cursor: pointer;
}

a {
    color: inherit;
    text-decoration: none;
}

img {
    max-width: 100%;
}

/* 3. Main Application Layout */

.app-container {
    display: flex;
    min-height: 100vh;
}

.main-content {
    flex: 1;
    min-width: 0;
    margin-left: var(--sidebar-width);
    padding: 30px 34px;
}

/* 4. Sidebar */

.sidebar {
    width: var(--sidebar-width);
    height: 100vh;
    position: fixed;
    top: 0;
    left: 0;
    background: var(--surface);
    border-right: 1px solid var(--border);
    padding: 26px 18px;
    display: flex;
    flex-direction: column;
    overflow-y: auto;
    z-index: 100;
}

.brand {
    display: flex;
    align-items: center;
    gap: 11px;
    padding: 0 10px;
    margin-bottom: 38px;
}

.brand-icon {
    width: 40px;
    height: 40px;
    background: var(--primary-light);
    color: var(--primary);
    border-radius: 12px;
    display: grid;
    place-items: center;
    font-size: 21px;
    font-weight: 700;
}

.brand-name {
    font-size: 19px;
    font-weight: 700;
    letter-spacing: -0.7px;
}

   font-size: 10px;
    font-weight: 700;
    color: #a2a8b8;
    letter-spacing: 1.2px;
    padding: 0 12px;
    margin-bottom: 10px;
}
