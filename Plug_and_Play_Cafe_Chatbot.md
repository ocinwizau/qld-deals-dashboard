# PLUG-AND-PLAY CAFÉ CHATBOT
## For Instagram DMs & Facebook Messenger

---

## 🤖 READY-TO-USE CHATBOT FLOWS

### 1. WELCOME / START FLOW
**Trigger:** User sends DM or opens Messenger chat

**Bot Message:**
```
Hey 👋 Welcome to [CAFE NAME]! I can help you with menu, bookings, or today's specials ☕

What would you like to do?
```

**Quick Replies / Buttons:**
- 📍 Location & Hours
- 🍽️ View Menu
- 🛒 Order Now
- 📅 Book a Table
- ☕ Today's Special
- ❓ Ask a Question

---

### 2. LOCATION & HOURS FLOW
**User clicks:** Location & Hours

**Bot Message:**
```
📍 We're located at: [Insert Address]

🕒 Opening Hours:
Mon–Fri: 6am–3pm
Sat–Sun: 7am–2pm

👉 Tap below for directions:
```

**Buttons:**
- 📍 Open in Google Maps
- ☎️ Call Café

---

### 3. MENU FLOW
**User clicks:** View Menu

**Bot Message:**
```
Here's our menu 👇 Let me know if you're after something specific!
```

**Buttons:**
- 📄 Full Menu (link)
- 🌱 Vegan Options
- 🥐 Breakfast
- ☕ Coffee

---

#### Subflow: Coffee
**User clicks:** Coffee

**Bot Message:**
```
Our coffee is a local favourite ☕

⭐ Best sellers:
- Flat White
- Iced Latte
- Cappuccino

Want to order ahead?
```

**Buttons:**
- 🛒 Order Now
- 📞 Call to Order

---

#### Subflow: Breakfast
**User clicks:** Breakfast

**Bot Message:**
```
🥐 BREAKFAST MENU ⭐

• Big Breakfast — $18.90
• Avocado Smash — $16.90
• Pancakes — $14.90
• Bacon & Eggs — $13.90
• Veggie Brekkie — $15.90

What's your pick? 👇
```

**Buttons:**
- 🛒 Order Now
- 📅 Book a Table

---

#### Subflow: Vegan Options
**User clicks:** Vegan Options

**Bot Message:**
```
🌱 VEGAN OPTIONS ⭐

We've got plenty of plant-based picks!

• Avocado Smash (vegan bread)
• Veggie Bowl
• Oat milk latte
• Fresh juices

Ask our staff what's fresh today! 🌿
```

**Buttons:**
- 🛒 Order Now
- ❓ Ask a Question

---

### 4. ORDER FLOW
**User clicks:** Order Now

**Bot Message:**
```
You can order ahead and skip the wait 👇
```

**Buttons:**
- 🛵 Order via Uber Eats
- 📱 Call to Order
- 📍 Visit In-Store

---

#### Subflow: Uber Eats
**User clicks:** Order via Uber Eats

**Bot Message:**
```
🛵 Great choice! 

Tap below to order on Uber Eats and skip the queue:

[UBER EATS LINK]

Usually ready in 20-30 mins 🚗
```

**Buttons:**
- 🛒 Track Order
- 📍 Get Directions

---

### 5. BOOKING FLOW
**User clicks:** Book a Table

**Bot Message:**
```
Sure! I can help with that 😊

How many people is the booking for?
```

**Collect:**
- Number of people

**Bot Message:**
```
Sweet! And which date works for you?
```

**Collect:**
- Date

**Bot Message:**
```
What time would you like?
```

**Collect:**
- Time

**Bot Message:**
```
Almost done! Your name and phone number please 🙌
```

**Collect:**
- Name
- Phone number

**Bot Message (Confirmation):**
```
Thanks [Name]! 🙌

Your booking:
👥 [X] people
📅 [Date]
🕒 [Time]

Our team will confirm shortly via SMS/phone.

See you soon! ☕🌟
```

---

### 6. TODAY'S SPECIAL FLOW
**User clicks:** Today's Special

**Bot Message:**
```
🔥 TODAY'S SPECIAL ⭐

[Insert Special Here]
Example: Coffee + Pastry Combo — $9.90

Limited stock today!

Want in? 👇
```

**Buttons:**
- 🛒 Order Now
- 📍 Get Directions
- ❓ Ask a Question

---

### 7. FAQ FLOW (Most Common Questions)

| Question | Bot Answer |
|----------|------------|
| Do you have WiFi? | Yes! Free WiFi available for all customers 😊 |
| Are you pet-friendly? | Yes! Pets are welcome in our outdoor seating area 🐶 |
| Gluten-free options? | Yes! Ask our staff for today's GF options 🌱 |
| Do you accept card? | Yes, we accept cash, card, and contactless 💳 |
| Are you open today? | We're open today! Come say hi ☕ |
| Parking? | Free parking out front! 🚗 |
| Can I book for tonight? | Sure! Tap "Book a Table" and we'll sort it 😊 |
| Kids menu? | Yes! Little ones eat free on weekends 👶 |

---

### 8. FALLBACK / HUMAN HANDOFF

**Trigger:** Bot doesn't understand user input

**Bot Message:**
```
I'm not 100% sure on that 🤔

Let me get someone from our team to help you!
```

**Buttons:**
- 📞 Call Café
- ✉️ Leave a Message

---

#### If user chooses "Leave a Message"
**Bot Message:**
```
Sure! Drop your question below and we'll get back to you ASAP 💬

Or give us a call: [PHONE NUMBER] ☎️
```

**Collect:**
- Message

**Bot Message:**
```
Thanks! We'll reply shortly 🙌

In the meantime — follow us for deals! 👇
```

---

### 9. LEAD CAPTURE FLOW
**Trigger:** After 2-3 interactions

**Bot Message:**
```
Want 10% OFF your next coffee? ☕

Drop your number and we'll send you deals & specials!

� text: [NUMBER]
📧 or email: [EMAIL]
```

**Collect:**
- Name
- Phone / Email

**Bot Message:**
```
AWESOME! 🙌

You're on the list! 🎉

Your 10% code will arrive via SMS shortly.

See you soon! ☕🌟
```

---

### 10. TONE & STYLE GUIDE

| Element | How to Use |
|---------|------------|
| 😄 Emoji | Use naturally, 1-2 per message |
| 📱 Short sentences | Keep under 20 words per line |
| 🙌 Local Aussie | "G'day", "no worries", "sorted" |
| 💬 Questions | End with "What do you reckon?" or "Sorted?" |
| ⭐ Upsell | Suggest add-ons: "Want a brownie with that?" |
| 🙋 Human | Use "I", "we're", "let me check" |

**Example Upsells:**
- "Want a brownie with that coffee? 🍫"
- "We have fresh croissants — want one?" 
- "Today's flat white is unreal ☕"

---

### 11. IMPLEMENTATION NOTES

#### Platform-Specific Notes:

| Platform | Implementation |
|----------|----------------|
| **ManyChat** | Use Flow Builder, add Quick Replies |
| **Botpress** | Create nodes matching each flow |
| **Chatfuel** | Use broadcast/automation features |
| **Tidio** | Use Canned Responses for FAQs |
| **WhatsApp Business** | Use quick replies + labels |

#### Key Buttons to Create:
- 📍 Location & Hours
- 🍽️ View Menu  
- 🛒 Order Now
- 📅 Book a Table
- ☕ Today's Special
- ❓ Ask a Question
- 📍 Open in Google Maps
- ☎️ Call Café
- 🛵 Order via Uber Eats
- 📞 Call to Order

---

### 📋 QUICK SETUP CHECKLIST

- [ ] Upload menu PDF/link
- [ ] Set opening hours in Location flow
- [ ] Add Google Maps link
- [ ] Add Uber Eats/delivery link
- [ ] Add booking link or form
- [ ] Test all FAQ responses
- [ ] Add phone number for Call to Order
- [ ] Set up lead capture (Google Sheets integration)
- [ ] Connect to FB Page & Instagram
- [ ] Go live! 🚀

---

### 💰 UPSELL OPPORTUNITIES

| Upsell | When to Trigger |
|--------|-----------------|
| Food add-ons | After ordering coffee |
| Loyalty program | After first purchase |
| Merchandise | After 3+ visits |
| Events/private hire | After booking |

---

### 🔧 TECHNICAL SETUP

**For Instagram/Facebook:**
1. Connect Page to ManyChat/Botpress
2. Enable Messenger + Instagram DM
3. Set up automatic responses
4. Test in Live mode

**For Website Widget:**
- Embed HTML chatbot OR
- Use Tawk.to / Tidio widget

---

## ✅ READY TO DEPLOY

This chatbot is optimized for:
- ✅ Converting interest to orders
- ✅ Capturing leads automatically
- ✅ Handling FAQs 24/7
- ✅ Sound friendly and local
- ✅ Drive bookings & repeat visits

---

**Now let's customize this for YOUR café!**

Reply with:
1. Your café name
2. Address
3. Phone number
4. Opening hours
5. Menu link
6. Uber Eats/link
7. Any specials you want to feature

I'll customize ALL the scripts with YOUR details! 🔴