# Dynamic Wedding Invitation

This project is a dynamic wedding invitation web page. The content (couple's names, event details, gallery, bank accounts, etc.) is loaded from a `data.json` file, making it easy to update without modifying the HTML structure.

## How to Run Locally

To view this invitation locally, you need to serve the files using a simple web server due to browser security policies (CORS).

1.  **Ensure Python is installed:**
    You likely already have Python installed. You can check by opening your terminal or command prompt and typing:
    ```bash
    python3 --version
    ```
    If it's not installed, please download it from [python.org](https://www.python.org/downloads/).

2.  **Navigate to the project directory:**
    Open your terminal or command prompt and go to the directory where `index.html` and `data.json` are located.
    ```bash
    cd /home/farhan/non_kerjaan/invitamu 
    ```
    (Replace `/home/farhan/non_kerjaan/invitamu` with the actual path if you move the project).

3.  **Start the local web server:**
    Run the following command to start a simple HTTP server:
    ```bash
    python3 -m http.server 8000
    ```
    This will start the server on port `8000`. You should see a message like `Serving HTTP on 0.0.0.0 port 8000 (http://0.0.0.0:8000/) ...`

4.  **Open in your browser:**
    Open your web browser (e.g., Chrome, Firefox) and navigate to:
    ```
    http://localhost:8000/index.html
    ```

## Customizing Content

All the dynamic content for the invitation is stored in `data.json`. You can edit this file to change:
*   Couple's names
*   Event dates and times
*   Venue details
*   Background video and images
*   Photo gallery
*   Bank account information
*   Love story timeline

Make sure to follow the JSON structure when making changes.

## Troubleshooting

*   **CORS Error (if opening `index.html` directly):** This is why you need to run the `python3 -m http.server` command. Opening `file:///.../index.html` directly will not work.
*   **Port already in use:** If port `8000` is already in use, you can try another port by running `python3 -m http.server 8080` (then access via `http://localhost:8080/index.html`).
