# 👑 NetworkPro | Network Marketing Hierarchy

A responsive network marketing genealogy website for managing members, tracking Personal Volume (PV), calculating team PV, and automatically determining level rates.

🌐 **Live Website:** https://shiva0909122.github.io/Network/

## 🚀 Features

- 📱 Fully responsive design for mobile, tablet, and desktop.
- 👥 Add, edit, and delete members.
- 🌳 Interactive genealogy tree showing upline and downline relationships.
- 🆔 Automatically generated member IDs.
- 📊 Track personal PV and total team PV.
- 🏆 Automatically calculate level rates based on total team PV.
- 🔄 Automatically update upline levels when downline PV changes.
- 🔍 Search members by name, ID, or sponsor.
- 💾 Store data in browser local storage.
- 📥 Export and restore data using JSON backups.
- 🌐 Static website with no database or backend required.

## 🏆 PV Level Structure

The level rate is calculated using the member's total team PV.

| Total Team PV | Level Rate |
|---:|---:|
| 0–599 PV | 5% |
| 600–2,399 PV | 8% |
| 2,400–5,499 PV | 12% |
| 5,500+ PV | 16% |

## 🌳 How Team PV Works

A member's Team PV includes:

- Their own personal PV.
- The PV of all direct downline members.
- The PV of all indirect downline members.

**Formula:**

Team PV = Own PV + Total PV from the entire downline.

### Example

Suppose Shiva has the following team:

| Member | Own PV |
|---|---:|
| Shiva | 200 |
| Rajj | 100 |
| Yyy | 400 |
| Yhb | 600 |
| **Total Team PV** | **1,300** |

Shiva's total Team PV is 1,300 PV.

According to the level structure, Shiva qualifies for the **8% level rate**.

If the team's total PV increases to 2,400 PV, Shiva qualifies for the **12% level rate**.

When PV changes for a member, the system should recalculate the total team PV and level rate for that member and every upline above them.

## 💻 Technology

- HTML5
- CSS3
- JavaScript
- Browser Local Storage
- D3.js for genealogy visualization
- Bootstrap for responsive styling

## 📱 How to Use

1. Open the live website.
2. Add a member by entering their name and PV.
3. Select their sponsor or upline.
4. Save the member.
5. View the updated genealogy tree.
6. Edit member details or PV whenever needed.
7. Monitor team PV and level rates.
8. Export backups regularly to protect your data.

## 💾 Data Storage

This application uses browser `localStorage` instead of a database.

- Data remains in the same browser profile on the same website origin.
- Data does not automatically synchronize between devices.
- Clearing browser storage may permanently delete saved members.
- Export JSON backups regularly to protect your information.

## ⚠️ Important Note

The percentages represent level qualification rates. They do not automatically represent commission payouts.

Actual commission calculations require a separately defined compensation plan.

## 🔗 Links

- **Live Website:** https://shiva0909122.github.io/Network/
- **GitHub Repository:** https://github.com/Shiva0909122/Network

## 📄 License

No license has been specified yet.
