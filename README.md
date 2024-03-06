# Insurance USSD Service with Africa's Talking

This is a USSD service built with Flask that provides information about different insurance products and allows users to:

1. **Browse**: Get information about various insurance types (Health, Motor, etc.) and the companies offering them.
2. **Contact**: Find contact information for specific insurance companies.
3. **Claim**: Initiate a claim process for Motor Insurance (Third-party and Own damage).

## README Contents

1. **Dependencies**: Required libraries and their purposes.
2. **Running the Application**: How to start the USSD service.
3. **Functionality**: Breakdown of the USSD interaction flow.
4. **SMS Integration**: Sending SMS notifications using Africa's Talking.

## Dependencies

- **Flask**: Microframework for building web applications.
- **Africa's Talking**: SDK for sending SMS and USSD interactions.

## Running the Application

1. Install dependencies: Run `pip install flask africastalking` in your terminal.
2. Configure Africa's Talking credentials: Replace the placeholders in the SMS class with your actual username and API key obtained from Africa's Talking.
3. Run the application: Execute `python app.py` in your terminal. This will start the USSD service on your local machine (default port 5000).

## Functionality

The application interacts with users through USSD menus and text inputs. It guides users through various options depending on their selections:

1. **Main Menu**: User selects the type of insurance they are interested in.
2. **Company Selection**: User chooses a specific company for the selected insurance type.
3. **Contact or Claim**:
   - **Contact**: Get the company's phone number for further inquiries.
   - **Claim (Motor Insurance only)**: Initiate a claim process by selecting the claim type (Third-party or Own damage) and providing necessary details like the vehicle number plate.

## SMS Integration

The application utilizes Africa's Talking SMS service to send notifications to users. Currently, it sends claim status updates and policy details upon request.

**Note**: This is a simplified example for illustrative purposes.
