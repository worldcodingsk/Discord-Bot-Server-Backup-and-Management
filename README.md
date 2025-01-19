# **Discord Bot – Server Backup and Management**

## **Popis**
Tento bot je navrhnutý na správu a zálohovanie Discord servera. Poskytuje funkcie na manuálne a automatické zálohovanie, obnovu databáz a správu blacklistu. Podporuje viacjazyčné prostredie a dynamickú nápovedu.

---

## **Funkcie**
### **Hlavné príkazy**
- **`!backup-server`**  
  - Vytvorí zálohu konfigurácie servera (roly, kanály, nastavenia).  
  - Súbor zálohy sa uloží vo formáte JSON.  
  - Prístup: **Administrátori**.  

- **`!backup`**  
  - Manuálne zálohuje databázu a odstraňuje staré zálohy.  
  - Prístup: **Administrátori**.  

- **`!restore`**  
  - Obnoví databázu zo zálohy, ak je dostupná.  
  - Prístup: **Administrátori**.  

- **`!blacklist <domain|keyword> <value>`**  
  - Pridá doménu alebo kľúčové slovo na blacklist.  
  - Prístup: **Administrátori**.  

- **`!help`**  
  - Zobrazí dynamický zoznam dostupných príkazov a automatických funkcií.  
  - Prístup: **Každý používateľ**.  

---

### **Automatické funkcie**
- Automatické zálohovanie databázy každých 24 hodín.  
- Odstraňovanie starých záloh (starších ako 30 dní).  
- Obnova databázy pri štarte bota, ak je poškodená alebo chýba.  
- Testovanie integrity šifrovaných záloh.  

---

## **Inštalácia**
1. Naklonujte repozitár:
   ```bash
   git clone https://github.com/worldcodingsk
   cd discord-bot
