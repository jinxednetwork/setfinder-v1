# setfinder-v1

# 🎬 SetFinder — Retro Studio Booking for Creators

**SetFinder** is a Bollywood-inspired web app for discovering and booking creative studios in Mumbai. Think Airbnb — but for podcasters, filmmakers, and content creators who want vibrant, aesthetic spaces full of desi charm.

Styled with grainy textures, fun fonts, and micro animations, it delivers a cinematic experience from search to booking.

---

## 🧑‍💻 User Story

As a Mumbai-based content creator, I want to:
- Browse available studios near me
- Filter by type: Podcast, Film, or Creator Loft
- View pricing, availability, and reviews
- Select add-ons like crew or gear
- Book my dream set with a flair of retro Bollywood style

No logins, no credit cards — just playful vibes and beautiful interfaces.

---

## 🚀 Features

### 🔍 Landing Page
- Hero section with a film-ticket styled search bar
- Inputs: Location, Dates, Studio Type (mocked)
- CTA: **"Find My Set!"** triggers **mock filtering** on featured studios
- Quirky subcopy: *“Your set. Your script. Book it.”*
- Category scroller with emojis (🎙️ 🎥 📸)
- Featured Studios grid with:
  - Studio thumbnail
  - Guest Favorite badge (styled like a film award)
  - Name, type, location
  - Price per hour/day
  - ❤️ Favorite button
  - Hover animations
  - Optional: **“Booked Out” overlay badge**

### 🏠 Studio Detail Page (`/studio/[slug]`)
- Full-width banner image
- Polaroid-style photo gallery (swipeable on mobile)
- Studio info + availability calendar (Shadcn)
- Description in a handwritten font
- Checkbox add-ons (producer, gear, etc.)
- Sticky CTA: **“Book This Studio”**
- **Review wall**:
  - Clapboard emoji avatars
  - Scrollable past reviews
  - Optional fan-message textarea

### 📅 Booking Page (`/book`)
- 3-step form with Bollywood-style copy:
  1. **“Lights… Dates… Book!”**
  2. **“Add Your Crew”** (add-ons)
  3. **“You’re Ready to Roll!”** (confirmation)
- Global state (via React Context) stores booking info
- Vertical stepper layout on mobile
- Fun CTA transitions and confetti effects (optional)

### ✅ Confirmation Page (`/confirmation`)
- Recap of selected dates, add-ons, and studio name
- Thank-you message with retro poster visuals

---

## 🛠 Tech Stack

- **Next.js** (TypeScript)
- **Tailwind CSS** for layout
- **Shadcn UI** for calendar and form components
- **Google Fonts** for retro typography
- **Static JSON** for mocked studio listings
- **React Context** to store booking flow data
- **Mobile-first responsive design**

---

## 🖼️ Visual Style Guide

- **Colors**: Maroon Red, Mustard Yellow, Deep Teal, Cream White
- **Fonts**:  
  - Headers: Bold Bollywood-style Serif  
  - Body: Rounded sans-serif
- **Design**:  
  - Grainy/paper textures  
  - Retro icons: clapperboard, camera, ticket stub  
  - Animated CTA buttons  
  - Hand-drawn borders

---

## 📦 Roadmap / Changelog

**v1 (MVP)**
- [x] Static JSON with 10 listings
- [x] Landing, detail, booking, confirmation pages
- [x] Mobile responsive
- [x] All booking mocked with local state

**Future Features**
- User login for creators
- Payments & real-time availability
- Studio owner dashboard
- Interactive map view
- Review submission + moderation

---

## 🧪 Testing Notes

- All booking and search are mocked
- Data resets on page refresh
- No backend or persistence in v1
