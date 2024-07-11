## Flask Application Design

### HTML Files

- **index.html**: The main page of the website, providing the user interface for making reservations. It will include a form with fields for the user's name, contact information, date, time, and group size.
- **confirmation.html**: A page displayed after a reservation is successfully submitted, providing a confirmation message and reservation details.

### Routes

- **home**: The route for the main page (`/`). It will render the `index.html` file.
- **reserve**: The route for processing the reservation request (`/reserve`). It will validate the user input, check availability, and save the reservation. If successful, it will redirect to the `confirmation.html` page; otherwise, it will redirect to the `index.html` page with error messages.
- **static**: The route for serving static files, such as CSS, JavaScript, and images (`/static/<filename>`).