Gym CRM: Elite Trainer Dashboard (MVP)
1. Visual Identity & "Boutique" Aesthetic
Theme: Elegant Minimalism (Anti-AI generated look).

Dark Mode: Pure Black (#000000) background, White text, Silver (#C0C0C0) strand accents/borders.

Light Mode: Pure White (#FFFFFF) background, Black text, Gold (#D4AF37) strand accents/pulses.

Typography: High-density data, generous letter spacing, clean Sans-Serif.

2. Navigation Architecture
Layout: Collapsible sidebar navigation that expands/contracts the main content area.

Breadcrumbs: Persistent header showing current module path (e.g., Clients > Add Client).

Modules:

Radar: Primary "at-risk" dashboard (formerly Ghosting Radar).

Clients (Master Menu): Dropdown with "All Clients" and "Add Client."

WhatsApp API: Placeholder (COMING SOON).

Payments: Placeholder (COMING SOON).

3. Core Logic & Validation
Ghosting Radar Sorting: Priority order: Red (Ghosting) > Amber (Slipping) > Dark Grey/Slate (Info Required) > Green (Active).

Info Required Status: Newly added clients like "Disha" default to Dark Grey until first health data sync.

Conditional Rendering: Health Intelligence charts (Recharts) are hidden if a client has no data or is in "Info Required" status.

Form Validation:

Mandatory Fields: Name, Phone, Email, Age, Weight, Gender, 3-hour Time Slot Window.

Regex: 10-digit Indian Phone (/^[6-9]\d{9}$/), Standard Email pattern.

4. Admin & Settings
Profile: Editable via top-right icon; takes user to /settings.

Gym Identity: Integrated Google Location API for gym address selection and Gym Name input.

5. Future Roadmap (18-Day Sprint)
Backend: Node.js/Express + Supabase for real-time data sync.

WhatsApp Bot: Twilio Sandbox for automated nudges and passive data extraction (Sleep, Steps, Mood).