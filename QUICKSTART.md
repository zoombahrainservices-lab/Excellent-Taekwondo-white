# ⚡ Quick Start Guide - Excellent Taekwondo Website

Get your website up and running in 10 minutes!

## 🎯 What You Have

A complete, modern, SEO-optimized static website with:
- ✅ 4 HTML pages (Home, About, Profile, Classes)
- ✅ Responsive CSS styling (Black, Red, White theme)
- ✅ Animated JavaScript interactions
- ✅ SEO optimization with meta tags and schema markup
- ✅ Mobile-friendly design

## 🚀 5-Minute Local Setup

### Step 1: Open the Website
Simply double-click `index.html` to open it in your default browser!

That's it for basic viewing.

### Step 2 (Optional): Use a Local Server
For better testing:

**Option A - Python** (if installed):
```bash
python -m http.server 8000
```
Then visit: `http://localhost:8000`

**Option B - Node.js** (if installed):
```bash
npx http-server
```

**Option C - VS Code**:
Install "Live Server" extension → Right-click `index.html` → "Open with Live Server"

## 📝 Essential Customizations

### 1. Add Your Phone Number (2 minutes)
Search and replace in ALL files:
- Find: `+973 XXXX XXXX`
- Replace with: Your actual phone number

- Find: `973XXXXXXXX` (WhatsApp link)
- Replace with: Your WhatsApp number (with country code, no spaces)

### 2. Add Your Email (1 minute)
- Find: `info@excellenttaekwondo.com`
- Replace with: Your actual email address

### 3. Add Pricing (2 minutes)
Open `classes.html`:
- Find: `BD XX`
- Replace with: Your actual prices (e.g., `BD 50`)

### 4. Update Social Media Links (2 minutes)
In ALL HTML files, find the social links section:
```html
<a href="#" class="social-link">
```
Replace `#` with your actual profile URLs:
- Facebook: `https://facebook.com/yourpage`
- Instagram: `https://instagram.com/yourprofile`
- YouTube: `https://youtube.com/@yourchannel`

## 🖼️ Adding Images

### Quick Method - Use Placeholders First
The website will work without images, but links will be broken.

### Proper Method - Add Your Images

1. **Create images folder** (if not exists):
   - Right-click in project folder
   - New Folder → Name it `images`

2. **Required images** (see `images/README.md` for details):
   - Hero backgrounds (5 images)
   - Class photos (9 images)
   - Instructor photos (4 images)
   - Gallery photos (6 images)
   - Social media images (2 images)

3. **Quick tip**: Use your phone to take photos of:
   - Training sessions
   - Instructors
   - The facility
   - Students in action (with permission!)

4. **Optimize before adding**:
   - Visit [tinypng.com](https://tinypng.com)
   - Upload and compress your images
   - Download and save to `images/` folder

## 🌐 Deploy to Internet (10 minutes)

### Easiest: Netlify (FREE)

1. Go to [netlify.com](https://netlify.com)
2. Sign up (free)
3. Drag your ENTIRE project folder to the upload area
4. Done! You get a free URL: `yoursite.netlify.app`

**Add Custom Domain** (if you have one):
- Settings → Domain Management → Add custom domain
- Follow DNS instructions from Netlify

See `DEPLOYMENT.md` for more detailed options.

## 📱 Test on Mobile

1. Deploy to Netlify (see above)
2. Open the URL on your phone
3. Test all pages and buttons
4. Try the WhatsApp button
5. Test the contact form

Everything should work smoothly on mobile!

## ✉️ Make Contact Form Work

Your form currently doesn't send emails. Choose one:

### Option 1: Formspree (Easiest - FREE)
1. Go to [formspree.io](https://formspree.io)
2. Sign up and create a form
3. Copy your form endpoint
4. In `index.html`, find the form tag
5. Change to:
```html
<form action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
```

### Option 2: Netlify Forms (if using Netlify)
In `index.html`, change form tag to:
```html
<form name="contact" method="POST" data-netlify="true">
```
Submissions will appear in your Netlify dashboard.

## 📊 Add Google Analytics (5 minutes)

1. Go to [analytics.google.com](https://analytics.google.com)
2. Create account and property
3. Get your tracking ID (G-XXXXXXXXXX)
4. Add this before `</head>` in ALL HTML files:

```html
<!-- Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=G-XXXXXXXXXX"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'G-XXXXXXXXXX');
</script>
```

Replace `G-XXXXXXXXXX` with your actual ID.

## 🎨 Customize Colors (Optional)

Open `styles.css` and find this at the top:
```css
:root {
    --primary-color: #E10600;    /* Red */
    --secondary-color: #000000;   /* Black */
    --white: #FFFFFF;             /* White */
}
```

Change the color codes to your preference!

## ✅ Launch Checklist

Before going live:

- [ ] Phone number updated everywhere
- [ ] Email updated
- [ ] WhatsApp link working
- [ ] Social media links added
- [ ] Pricing information added
- [ ] Images uploaded (or placeholders working)
- [ ] Contact form connected
- [ ] Tested on mobile phone
- [ ] Tested on desktop browser
- [ ] Deployed to internet
- [ ] Analytics installed (optional)

## 🆘 Common Issues

### "Images not showing"
- Check that `images` folder exists
- Verify image filenames match HTML (case-sensitive!)
- Try using lowercase filenames only

### "WhatsApp button not working"
- Remove spaces from phone number in link
- Format: `https://wa.me/973XXXXXXXX`
- Include country code (973 for Bahrain)

### "Form not submitting"
- Set up Formspree or Netlify Forms (see above)
- Default form won't work without backend

### "Website looks broken on mobile"
- It's already responsive! Make sure you deployed it properly
- Clear browser cache
- Try different mobile browsers

## 📚 Need More Help?

- **Detailed deployment**: See `DEPLOYMENT.md`
- **Image guidelines**: See `images/README.md`
- **Full documentation**: See `README.md`

## 🎉 You're Done!

Your website is ready to launch! 

### Next Steps:
1. Add your images
2. Deploy to Netlify
3. Share with your students
4. Promote on social media
5. Add to Google My Business

---

**Need professional help?** Consider hiring a web developer for:
- Professional photography
- Custom features
- Advanced form handling
- Payment integration
- Booking system

**The website is designed to be easy to maintain!** You can update text content directly in the HTML files using any text editor.

---

*Built for Excellent Taekwondo - Discipline. Strength. Excellence.* 🥋

