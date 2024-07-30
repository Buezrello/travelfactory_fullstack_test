# Backend and Frontend projects for TravelFactory test.

### The backend run by default in http://localhost:8080 and waiting requests from a frontend.

### The frontend can be start with "npm start" and by default run on http://localhost:3000

## The frontend send requests to backend to http://localhost:8080

For now the value hardcoded in a package.json:
"proxy": "http://localhost:8080"

It can be changed for a real deployment.

### I'm afraid I got a little confused in the requirements and maybe didn't do exactly what was required of me.
But the general idea is correct. I created a component for editing translation map too but because there is no such button on your screenshot I disabled it, it can be enabled in a future if need.

### The application working this way now.
1. The button "Add app": opens a pop-up window where you can create a new application, put manually Last deployment date/time and add translations in form key/value
2. The created application added to a right site of a screen in a card form and the name of the application added to a left side of a screen.
3. Every card on the right side of the screen have two buttons, "Download on XLSX" and "Deploy"
4. The button "Download on XLSX download the Excel with translation to a default browser download directory".
5. The button "Deploy" deploying the translation in JSON format to a server, into the directory configured in a backend. By default, it's a subdirectory "translation" in a working directory, but it can be changed by setting an environment variable TRANSLATION_JSON_DIRECTORY
