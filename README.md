# Finance Newsletter Re Engagement Email Template

Professional Finance Newsletter providing valuable insights and updates on market trends.

![Thumbnail](./thumbnail.png)

## Template Details

- **Industries:** Finance
- **Message Type:** Newsletter
- **Tags:** financial_update, market_trends, economic_insights

## Files
- `index.html`: The improved, localized, and branded HTML template.
- `template.blade.php`: Ready-to-use Laravel Blade template with `asset()` helpers.
- `assets/`: Directory containing localized images and styles used in the template.

## Usage in Laravel

### 1. Store the Template
Place the `index.html` content in a Blade view (e.g., `resources/views/emails/Finance-newsletter-re-engagement-email-template.blade.php`).

### 2. Handle Assets
Move the content of `assets/` to your public directory (e.g., `public/vendor/mail-templates/Finance-newsletter-re-engagement-email-template/`) and update the paths in the HTML to use the `asset()` helper.

### 3. Send Email
```php
Mail::to($user)->send(new \App\Mail\GenericEmail([
    'view' => 'emails.Finance-newsletter-re-engagement-email-template',
    'data' => [
        // Your dynamic data here
    ]
]));
```

---
*Created with ❤️ by **[LaravelMail.com](https://laravelmail.com)** - Your source for professional email templates.*
