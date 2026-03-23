# Contact Form Setup Guide

## EmailJS Configuration

1. **Create an EmailJS account** at [emailjs.com](https://www.emailjs.com/)

2. **Create an email service**:
   - Go to Email Services in your dashboard
   - Connect your email provider (Gmail, Outlook, etc.)
   - Note down the Service ID

3. **Create an email template**:
   - Go to Email Templates
   - Create a template with these variables:
     - `{{from_name}}` - Sender's name
     - `{{from_email}}` - Sender's email
     - `{{subject}}` - Email subject
     - `{{message}}` - Message content
   - Set the recipient email to your email address
   - Note down the Template ID

4. **Get your Public Key**:
   - Go to Account → General
   - Copy the Public Key

5. **Update environment variables** in `.env.local`:
   ```
   NEXT_PUBLIC_EMAILJS_SERVICE_ID=your_actual_service_id
   NEXT_PUBLIC_EMAILJS_TEMPLATE_ID=your_actual_template_id
   NEXT_PUBLIC_EMAILJS_PUBLIC_KEY=your_actual_public_key
   ```

## reCAPTCHA Configuration

1. **Get reCAPTCHA keys** at [Google reCAPTCHA](https://www.google.com/recaptcha/admin)

2. **Create a new site**:
   - Choose reCAPTCHA v2 "I'm not a robot" Checkbox
   - Add your domain (localhost for development)
   - Note down the Site Key

3. **Update environment variable** in `.env.local`:
   ```
   NEXT_PUBLIC_RECAPTCHA_SITE_KEY=your_actual_site_key
   ```

## Calendly Setup (Optional)

1. **Create a Calendly account** at [calendly.com](https://calendly.com/)

2. **Set up your availability**:
   - Configure working hours (Weekdays 10 AM - 6 PM IST)
   - Create event types for different meeting purposes

3. **Update the Calendly link** in `contact-section.tsx`:
   ```typescript
   href: 'https://calendly.com/your_actual_username'
   ```

## Testing the Form

1. **Restart the development server** after updating environment variables
2. **Test the form** with valid data and reCAPTCHA verification
3. **Check your email** for received messages
4. **Test validation** with invalid inputs

## Security Notes

- Never commit `.env.local` to version control
- The reCAPTCHA helps prevent spam submissions
- EmailJS handles server-side email sending securely
- All form data is validated on both client and server side