# OBS Zoom to Mouse (Fixed for Modern OBS)

A fixed version of the popular `obs-zoom-to-mouse.lua` script for OBS Studio.

This version resolves the runtime crash error on **line 435** (`attempt to call field 'obs_sceneitem_get_info' a nil value`) caused by API changes in OBS Studio 28 and newer releases.

---

## 🚀 How to Install & Download

1. Click on `obs-zoom-to-mouse-fixed.lua` above, then click the **Download raw file** button (or right-click [here](https://raw.githubusercontent.com/PavanKumarGS223/obs-zoom-to-mouse-fixed/main/obs-zoom-to-mouse-fixed.lua) and select **Save link as...**).
2. Save the file to a known folder on your PC.
3. Open **OBS Studio**.
4. Go to **Tools** → **Scripts**.
5. Click the **`+` (Plus)** icon in the bottom left.
6. Select `obs-zoom-to-mouse-fixed.lua` and click **Open**.

---

## ⚙️ How to Setup

1. In OBS, right-click your **Display Capture** (or Screen Capture) source and select **Filters**.
2. Click the **`+`** icon under **Effect Filters** and add **Zoom to Mouse**.
3. Go to **OBS Settings** → **Hotkeys** to assign a hotkey to toggle zoom on/off.

---

## 🛠️ What Was Fixed?

* Replaced deprecated `obs_sceneitem_get_info` with `obs_sceneitem_get_info2` on line 435 to support modern OBS C API bindings.
