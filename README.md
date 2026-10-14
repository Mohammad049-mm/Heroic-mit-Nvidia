---

## Heroic Games Launcher: NVIDIA-Optimierungen

Diese Umgebungsvariablen (Environment Variables) optimieren die Performance und Features beim Spielen über den Heroic Games Launcher auf Systemen mit NVIDIA-Grafikkarten.

### Variablen im Heroic Launcher hinzufügen:

Trage die folgenden Schlüssel-Wert-Paare in den Einstellungen des jeweiligen Spiels unter **Umgebungsvariablen** (Environment Variables) ein:

#### 1. Nutzung der NVIDIA-GPU erzwingen
Verhindert, dass das Spiel versehentlich auf einer integrierten Intel- oder AMD-Grafikeinheit (iGPU) startet:
* **Schlüssel:** `DXVK_FILTER_DEVICE_NAME`
* **Wert:** `NVIDIA`

#### 2. NVIDIA-Features aktivieren (z. B. DLSS)
Schaltet die Unterstützung für die NVIDIA NVAPI frei, welche zwingend für Features wie DLSS (Deep Learning Super Sampling) und Raytracing unter Proton benötigt wird:
* **Schlüssel:** `PROTON_ENABLE_NVAPI`
* **Wert:** `1`
