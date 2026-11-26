# Learning diary, TJTP1140 Enterprise Information Systems

Sami Mäkelä, autumn 2026. 
Teacher José Teixeira, assistant Loviisa Hurme.

---

## Week 1

**Wed 28.10, intro.** Was there. Introductions, syllabus walkthrough, and Mentimeter votes on how the course runs. We picked Zoom for remote teaching, recordings for everyone, students forming their own video groups, textbook chapters as pre-reading and 23:59 deadlines.

**Thu 29.10, ERP and CRM.** Missed it. Went through the slides afterwards. ERP is the back office with one shared database. CRM is the front office for customers and sales. Covered ERP history from MRP to cloud, the market (SAP and Oracle, Salesforce leading CRM) and Lidl as a failure. Lidl spent around €500M on SAP and dropped it because it customised the system to fit its own way of working instead of changing its processes. Main point was that it's rarely the software. Hands-on part was a shared surf shop in Dolibarr where everyone added a supplier and a product. Skipped that since I wasn't there. The Dolibarr work for me came later with Hands-on Ex. 1.

---

## Week 2

**Wed 4.11, ERP and CRM foundations.** Turned out the class was replaced with three videos and two Moodle forum tasks, which I didn't notice in time. Videos were one on ERP history from MRP onwards (Brain Blitz Audios), Eric Kimberling on conflicts of interest between ERP vendors, consultants and buyers, and the Norwegian Consumer Council's A Day in the Life of an Enshittificator. Answered the first forum question on whether open source ERP removes Kimberling's conflict of interest. My answer was that it mostly moves it. Odoo partners still earn from Enterprise subscriptions and migrations, and the four freedoms make it easier to switch consultants but don't make the work free. Didn't comment on a peer's post in time and missed the enshittification forum.

**Thu 5.11, SQL.** Remote lecture on Zoom. Covered where SQL came from: navigational databases before 1970, Codd's relational model, SEQUEL at IBM renamed to SQL, Oracle shipping before IBM. SQL is declarative, you say what you want and the database works out how. SELECT, WHERE, ORDER BY and GROUP BY do most of the work. After that a Gimkit quiz game on the course so far, but the session ended early. The rest was meant to be self-paced with the w3schools SQL tutorial and the course Dolibarr database in phpMyAdmin. Skipped the tutorial since I took a databases course over the summer and SQL is familiar.

---

## Week 3

Had the flu for just over a week, so missed both sessions. Neither was recorded.

**Wed 11.11, Alban et al. chapters 4 to 6.** Went through the slides afterwards. They had the exam info and the guest lecture schedule, then the chapters. Ch. 4 on charting the organisation, a map is never the territory. Ch. 5 on planning the IS like a city, with weak links between blocks and strong ties inside them, and the IS shanty town when nobody does. Ch. 6 on extended vs cooperative IS, cloud and lock-in.

**Thu 12.11, web services behind e-commerce.** Went through the slides at home. How a click on Buy reaches the ERP through the shop, payment provider and carrier APIs. HTTP requests and responses, REST, JSON, status codes, API keys, webhooks. Skipped the curl examples at the end and used the API from Python later for Hands-on Ex. 3.

**Other work:**
- Theoretical Ex. 1A on Mon 9.11. Went to Prisma Seppälä and used the Kerää ja skannaa self-checkout, scanning with the S-ostoslista app and paying at the register with S-mobiili. Drew it as a PlantUML sequence diagram, including the staff steps for the age-restricted item check and discount items. Returned it the same day.
- Hands-on Ex. 1 on Mon 9.11 in the Dolibarr UI. Product Sami_Makela_surfboard, business customer Sami_Makela_in_JKL, a validated sales order for 5 units and a standard invoice from it. 2,500.00 EUR excl. tax, 3,125.00 EUR incl. 25% VAT. Returned the invoice PDF.
- Hands-on Ex. 2 on Wed 11.11. Answered the business questions with SQL in phpMyAdmin: products for sale, customer invoices, and stock per open warehouse.

---

## Week 4 (due Sat 21.11)

Back on campus for the guest lectures. Went to all four.

**Wed 18.11, guest lectures.** Santeri Pohjakallio from Ceili, a Salesforce consultancy, on CRM systems, CRM implementation projects and how AI changes both. CRM is people, processes and technology together. Projects run on the iron triangle of budget, schedule and scope, with the vendor selling licences, a partner implementing and the customer adopting. The old way is one UI per task with the user as the glue between systems. The new way is an AI assistant in the middle connected to CRM, ERP, email and documents through MCP, with the same permissions still applying. Most project problems aren't technical. Aleksanteri Strömberg from Accenture on SAP and testing. He covered a test automation tool for SAP, can't remember the name.

**Thu 19.11, guest lectures.** Loviisa Hurme from JYU on IT procurement in the public sector and the different tendering procedures. Janne Kallunki from Cloudpermit, a permit application system spun off from a state project done with Solita. Built in Clojure, and now expanding into North America.

**Other work:**
- Theoretical Ex. 2 on Sun 15.11. Compared an ERP video (ERPNext, Odoo, Dolibarr and SAP) with a Salesforce CRM tutorial through screenshots, looking at what data each system holds and how it's used.
- Hands-on Ex. 3 on Thu 19.11 and Fri 20.11. Two Python scripts against the Dolibarr REST API with an API key in the headers. One lists customers with unpaid invoices and the total owed, which needs a second call per invoice to get the customer name from its ID. The other creates Nordic Supply Oy as a new customer and reads it back to check the fields saved. Used Claude for help and said so in the README.
- Group video, done solo with the teacher's OK. On Nissen, Wienand and Schuette (2023), I See No Fun in Enterprise Systems, about users' first impressions of enterprise system UX. Wrote the script, filmed on campus Wed 18.11 and Thu 19.11, edited Thu and Fri, and submitted it Sat 21.11.

---

## Week 5 (due Sat 28.11)
**Wed 25.11, open source governance and ERP research.** Was there. Three of the teacher's research talks, covered quickly. One on Odoo: how OpenERP went open core in 2015 with a contributor agreement, a weaker licence and a paid Enterprise edition, and what happened to outside developers. First numbers show 75% of them stopped contributing to the core after the change. One on PyTorch moving from Meta to the Linux Foundation in 2022. More outside organisations and independent developers joined, but institutional developers went down, so breadth is not depth. One on TensorFlow and the roles of universities, research institutes and foundations, which sit at the edge of the network but do different jobs. Readings were Pekkola et al. (2013) on ERP research being mostly about implementation, and Kähkönen et al. (2017) on ERP development networks, where challenges split into triggers, root causes and consequences.

**Thu 26.11, exam.** Took the exam. Went aight.

**Other work:**

Theoretical Ex. 1B on Thu 26.11 after the exam. Revisited the Prisma self-checkout diagram and added the backend systems behind the register: API, ERP, CRM and loyalty, and payment. Plus notes on how and why it changed.
