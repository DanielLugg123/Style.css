:root {
    --primary: blue;
    --secondary: yellow;
    --background: white;
    --text: red;
    --font-main: Times New Roman, Italic;
}

body {
    margin: 0;
    font-family: var(--font-main);
    background: var(--background);
    color: var(--text);
}

.container {
    width: 95%;
    margin: auto;
}

header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    background: var(--primary);
    padding: 15px;
}

nav ul {
    list-style: none;
    display: flex;
    gap: 15px;
}

nav a {
    text-decoration: none;
    color: white;
}

nav a:hover {
    color: var(--secondary);
    transition: 0.3s ease;
}

.hero {
    text-align: center;
    padding: 40px;
    background: var(--secondary);
    color: white;
}

section {
    margin: 20px 0;
    padding: 20px;
    border: 1px solid var(--primary);
}

.card {
    background: white;
    padding: 15px;
    margin: 10px 0;
}

.card:hover {
    transform: scale(1.02);
    transition: 0.3s ease;
}

table {
    width: 100%;
    border-collapse: collapse;
}

th, td {
    border: 1px solid var(--primary);
    padding: 10px;
}

footer {
    text-align: center;
    padding: 20px;
    background: var(--primary);
    color: white;
}

/* Responsive */

@media (min-width: 600px) {
    #resume {
        display: flex;
        flex-direction: column;
    }
}

@media (min-width: 950px) {
    #resume {
        display: grid;
        grid-template-columns: repeat(2, 1fr);
        gap: 20px;
    }
}
