✈️ TravelGo - 
A full-stack travel booking web application built with Flask and AWS that allows users to book buses, trains, flights, and
hotels — with real-time booking confirmation via AWS SNS.

✨ Features - 
  🔐 **User Registration & Login** — Secure session management
  🚌 **Bus, 🚆 Train, ✈️ Flight & 🏨 Hotel Booking** — All travel needs in one place
  💺 **Seat Selection Interface** — Choose your preferred seat
  💳 **Payment Processing** — Method and reference tracking
  🎫 **Ticket Generation** — Instant ticket after successful booking
  📧 **Real-Time Confirmation** — Booking alerts via AWS SNS (email/SMS)
  📊 **User Dashboard** — View and manage all past bookings

🛠️ Tech Stack - 
| Layer | Technology |

| Backend | Python, Flask |
| Frontend | HTML, CSS (Jinja2 Templates) |
| Database | AWS DynamoDB |
| Notifications | AWS SNS |
| Cloud | AWS (EC2, DynamoDB, SNS) |

📁 Project Structure - 
  TravelGo/
   └── zoroo/
   ├── app.py                 
   └── templates/
   ├── index.html       
   ├── login.html         
   ├── register.html      
   ├── dashboard.html     
   ├── bus.html          
   ├── train.html         
   ├── flight.html        
   ├── hotels.html        
   ├── seat.html          
   ├── payment.html      
   └── ticket.html
---

⚙️ Setup & Installation - 

### Prerequisites

- Python 3.8+
- AWS Account with DynamoDB and SNS configured
- AWS CLI configured with credentials

### Steps

**1. Clone the repository**
```bash
git clone https://github.com/your-username/TravelGo.git
cd TravelGo/zoroo
```

**2. Install dependencies**
```bash
pip install flask boto3
```

**3. Set environment variables**
```bash
export FLASK_SECRET_KEY="your-secret-key-here"
export AWS_REGION="ap-south-1"
```

**4. AWS Setup**
- Create a DynamoDB table named `Travel_user` with `email` as the partition key
- Create a DynamoDB table named `bookings` with a GSI named `email-index`
- Create an SNS topic and update the `SNS_TOPIC_ARN` in `app.py`

**5. Run the application**
```bash
python app.py
```
Visit `http://localhost:5000` in your browser

📋 Requirements - 
    flask
    boto3

Author - 
Harinitha V.N
B.Tech [Computer Science and Business Systems]
SSM Institute of Engineering and Technology, Dindigul
