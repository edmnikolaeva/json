# REST API Design - HTTP Request & Response 

<table>
<tr>
<td>

This repository shows a practical example of REST API design for the "Partners" screen in the mobile app of the online grocery store.  
The endpoint delivers structured partner store data (logos, delivery info, external links) to power clickable partner cards.
API design demonstrates how backend services interact with the frontend.

</td>
<td width="220">
<img src="https://github.com/edmnikolaeva/json/blob/main/json_sample.png" 
     alt="Visual Anchor — Main Screen Prototype" 
     width="200"/>
</td>
</tr>
</table>

---

### 🧩 Main Artifacts

- 👉 [HTTP request](https://github.com/edmnikolaeva/json/blob/main/get_partners_request.json)
- 👉 [HTTP response](https://github.com/edmnikolaeva/json/blob/main/get_partners_response.json)

---

### 🧭 Business Context

- **Domain:** online grocery delivery & marketplace
- **Scope:** partner storefront discovery 
- **Feature:** new "Partners" screen in mobile app — showcases cooperating physical stores
- **Goal:** enable quick transition to partner websites for in-store pickup, promotions or additional shopping

---

### 💼 Business Value

- Improved partner visibility in the app → more assortment & pickup points  
- Increase user convenience → hybrid online/offline experience  
- Drive cross-traffic to physical stores → higher overall loyalty & revenue potential

---

### ⚙️ Technical Notes

- Protocol: HTTP REST  
- Data format: JSON  
- Method: GET  
- Response: `200 OK` with partner collection  
- Each partner includes external deep link

---

### 👩‍💼 My Role 

- Analyzed screen mockup and business need  
- Designed minimal REST endpoint: `GET /v1/partners`  
- Defined request headers (Accept, User-Agent)  
- Structured response schema matching UI cards:  
  - `id` — unique identifier  
  - `name` — store brand  
  - `delivery_info` — polymorphic (time window or fast delivery)  
  - `logo_url` — CDN-hosted image  
  - `external_url` — deep link for transition  
- Provided production-like JSON examples for frontend integration

---

### 🔗 Related Artifacts

- 👉 [REST](https://github.com/edmnikolaeva/rest)
- 👉 [XML & SOAP](https://github.com/edmnikolaeva/xml)
- 👉 [Architecture](https://github.com/edmnikolaeva/architecture) 
- 👉 [C4 Model](https://github.com/edmnikolaeva/C4)
 
