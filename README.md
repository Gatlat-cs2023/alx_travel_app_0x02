## Payment Integration with Chapa

### Endpoints
- **Initiate Payment**: `POST /api/bookings/{booking_id}/payments/initiate/`
- **Verify Payment**: `GET /api/payments/{transaction_id}/verify/`
- **Webhook**: `POST /api/payments/webhook/`

### Environment Variables
- `CHAPA_SECRET_KEY`: Your Chapa API secret key
- `CHAPA_BASE_URL`: Chapa API base URL (https://api.chapa.co/v1)
- `CHAPA_WEBHOOK_URL`: Your webhook URL for payment notifications
- `FRONTEND_URL`: Your frontend URL for redirection after payment

### Testing
Use Chapa's sandbox environment for testing payments. Set `CHAPA_BASE_URL` to `https://api.chapa.co/v1` for production.