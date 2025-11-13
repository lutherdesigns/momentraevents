
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>MoMentra Events - Book MC Kudzi</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            min-height: 100vh;
            padding: 20px;
        }

        .container {
            max-width: 700px;
            margin: 0 auto;
            background: white;
            border-radius: 20px;
            box-shadow: 0 20px 60px rgba(0,0,0,0.3);
            overflow: hidden;
        }

        .header {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
            padding: 40px 30px;
            text-align: center;
        }

        .header h1 {
            font-size: 2.5em;
            margin-bottom: 10px;
            font-weight: 700;
        }

        .header .tagline {
            font-size: 1.1em;
            opacity: 0.95;
            font-style: italic;
        }

        .header .mic-icon {
            font-size: 3em;
            margin-bottom: 15px;
        }

        .form-content {
            padding: 40px 30px;
        }

        .form-intro {
            text-align: center;
            margin-bottom: 30px;
            color: #333;
        }

        .form-intro p {
            font-size: 1.05em;
            line-height: 1.6;
        }

        .form-group {
            margin-bottom: 25px;
        }

        label {
            display: block;
            margin-bottom: 8px;
            color: #333;
            font-weight: 600;
            font-size: 0.95em;
        }

        input[type="text"],
        input[type="email"],
        input[type="tel"],
        input[type="date"],
        select,
        textarea {
            width: 100%;
            padding: 12px 15px;
            border: 2px solid #e0e0e0;
            border-radius: 8px;
            font-size: 1em;
            transition: all 0.3s ease;
            font-family: inherit;
        }

        input:focus,
        select:focus,
        textarea:focus {
            outline: none;
            border-color: #667eea;
            box-shadow: 0 0 0 3px rgba(102, 126, 234, 0.1);
        }

        textarea {
            resize: vertical;
            min-height: 120px;
        }

        .required {
            color: #e74c3c;
        }

        .submit-btn {
            width: 100%;
            padding: 15px;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
            border: none;
            border-radius: 8px;
            font-size: 1.1em;
            font-weight: 600;
            cursor: pointer;
            transition: transform 0.2s ease, box-shadow 0.2s ease;
        }

        .submit-btn:hover {
            transform: translateY(-2px);
            box-shadow: 0 10px 25px rgba(102, 126, 234, 0.4);
        }

        .submit-btn:active {
            transform: translateY(0);
        }

        .event-types {
            display: grid;
            grid-template-columns: 1fr;
            gap: 10px;
            margin-top: 10px;
        }

        .footer {
            text-align: center;
            padding: 20px;
            background: #f8f9fa;
            color: #666;
            font-size: 0.9em;
        }

        .success-message {
            display: none;
            background: #d4edda;
            color: #155724;
            padding: 15px;
            border-radius: 8px;
            margin-bottom: 20px;
            border: 1px solid #c3e6cb;
        }

        @media (max-width: 600px) {
            .header h1 {
                font-size: 2em;
            }
            
            .form-content {
                padding: 30px 20px;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="header">
            <div class="mic-icon">🎤</div>
            <h1>MoMentra Events</h1>
            <p class="tagline">Moments That Move You</p>
        </div>

        <div class="form-content">
            <div class="form-intro">
                <p><strong>Book MC Kudzi for Your Special Moment</strong></p>
                <p>The voice your event deserves • Now booking 2025–2026</p>
            </div>

            <div id="successMessage" class="success-message">
                Thank you for your booking request! We'll get back to you within 24 hours.
            </div>

            <form id="bookingForm" action="https://formsubmit.co/bookmomentraevents@gmail.com" method="POST">
                <!-- FormSubmit Configuration -->
                <input type="hidden" name="_subject" value="New MoMentra Events Booking Request">
                <input type="hidden" name="_captcha" value="false">
                <input type="hidden" name="_template" value="table">
                
                <div class="form-group">
                    <label for="name">Full Name <span class="required">*</span></label>
                    <input type="text" id="name" name="name" required>
                </div>

                <div class="form-group">
                    <label for="email">Email Address <span class="required">*</span></label>
                    <input type="email" id="email" name="email" required>
                </div>

                <div class="form-group">
                    <label for="phone">Phone Number <span class="required">*</span></label>
                    <input type="tel" id="phone" name="phone" required>
                </div>

                <div class="form-group">
                    <label for="eventType">Event Type <span class="required">*</span></label>
                    <select id="eventType" name="event_type" required>
                        <option value="">-- Select Event Type --</option>
                        <option value="Wedding">Wedding</option>
                        <option value="Engagement">Engagement</option>
                        <option value="Birthday">Birthday</option>
                        <option value="Anniversary">Anniversary</option>
                        <option value="Graduation">Graduation</option>
                        <option value="Send-Off">Send-Off</option>
                        <option value="Baby Dedication">Baby Dedication</option>
                        <option value="Youth Revival">Youth Revival</option>
                        <option value="Conference">Conference</option>
                        <option value="Book Launch">Book Launch</option>
                        <option value="Charity Gala/Fundraiser">Charity Gala/Fundraiser</option>
                        <option value="Award Ceremony">Award Ceremony</option>
                        <option value="Other">Other</option>
                    </select>
                </div>

                <div class="form-group">
                    <label for="eventDate">Event Date <span class="required">*</span></label>
                    <input type="date" id="eventDate" name="event_date" required>
                </div>

                <div class="form-group">
                    <label for="eventTime">Event Time</label>
                    <input type="text" id="eventTime" name="event_time" placeholder="e.g., 2:00 PM - 6:00 PM">
                </div>

                <div class="form-group">
                    <label for="venue">Event Venue/Location <span class="required">*</span></label>
                    <input type="text" id="venue" name="venue" placeholder="City and venue name" required>
                </div>

                <div class="form-group">
                    <label for="guestCount">Expected Number of Guests</label>
                    <input type="text" id="guestCount" name="guest_count" placeholder="Approximate number">
                </div>

                <div class="form-group">
                    <label for="details">Additional Details</label>
                    <textarea id="details" name="additional_details" placeholder="Tell us more about your event, special requirements, or any questions you have..."></textarea>
                </div>

                <div class="form-group">
                    <label for="hearAbout">How did you hear about us?</label>
                    <select id="hearAbout" name="hear_about">
                        <option value="">-- Select --</option>
                        <option value="Social Media">Social Media</option>
                        <option value="Friend/Family Referral">Friend/Family Referral</option>
                        <option value="Previous Event">Attended Previous Event</option>
                        <option value="Google Search">Google Search</option>
                        <option value="Other">Other</option>
                    </select>
                </div>

                <button type="submit" class="submit-btn">Submit Booking Request</button>
            </form>
        </div>

        <div class="footer">
            <p><strong>MoMentra Events</strong> | Hosting with elegance & energy</p>
            <p>📧 bookmomentraevents@gmail.com</p>
            <p style="margin-top: 10px; font-style: italic;">#MomentraMoments</p>
        </div>
    </div>

    <script>
        document.getElementById('bookingForm').addEventListener('submit', function(e) {
            // Form will submit naturally to FormSubmit
            // Optional: Show loading state
            const btn = this.querySelector('.submit-btn');
            btn.textContent = 'Sending...';
            btn.disabled = true;
        });
    </script>
</body>
</html>
