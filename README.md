# 📷 ZedBoard + D5M Camera | “What’s in a Name?”

This is a small FPGA camera project I worked on in Tucson around 2018.  
It combines a **Terasic D5M 5MP camera sensor** and a **Xilinx ZedBoard** to capture raw images and display them live — with an unexpected moment that made it special.

<p align="center">
  <img src="https://github.com/zakinder/zedboard-d5m-name-echo/blob/main/images/20181021_223703.jpg" alt="WHAT'S IN A NAME?" width="600"/>
</p>

---

## 🔍 Project Summary

I connected the D5M camera to the ZedBoard (which has a Zynq-7000 SoC combining an FPGA and ARM processor).  
The goal: capture raw pixel data, send it through the FPGA logic, and display it on a monitor in real time.

One interesting moment: during a test, my camera happened to pick up a TV screen that showed the phrase **“WHAT’S IN A NAME?”**  
This wasn’t planned — just a pure **coincidence** that happened naturally, frozen in the raw frame along with the sensor’s pixel noise.

---

## ⚙️ How It Works

- **Hardware**
  - Terasic D5M CMOS Camera (MT9P031)
  - Xilinx ZedBoard (Zynq-7000 SoC)

- **FPGA Logic**
  - Camera sensor interface
  - Region of Interest (ROI) selection
  - Basic frame buffer for live video output
  - Simple text overlay

- **Output**
  - VGA or HDMI display showing raw sensor feed (with or without overlays)

---

## 💡 Why This Matters

This project is about more than pixels and hardware — it’s about how **real signals and meaning appear in natural time**.

The phrase *“WHAT’S IN A NAME?”* showed up by chance while I was testing hardware — not planned, not staged.  
It reminded me that a name is just a label — the truth is hidden deeper, in the raw data and real time flow.

Sometimes, even in FPGA pipelines, **truth leaks through at exactly the right moment** — if you’re paying attention.

---

## 📂 Project Structure

/src/fpga/         # HDL for sensor interface & ROI windowing  
/src/ps/           # Zynq PS software (if needed)  
/constraints/      # ZedBoard XDC pin mappings  
/docs/             # Design notes  
/images/test_frames/  # Example raw frames  
README.md

---

## ✅ What You Can Do

- Learn how to hook a simple camera module to an FPGA.
- Try raw pixel capture and ROI windowing.
- Experiment with overlaying text or graphics.
- Remember: sometimes the **natural flow of time** gives you the best signals.

---

## 🔓 License

Open source under MIT — fork it, adapt it, or build your own hidden frames.

---

## ✨ Contact

This was part of my own learning and reflection.  
If you’d like to discuss FPGA cameras, ZedBoard work, or the deeper story behind *“WHAT’S IN A NAME?”* — feel free to open an issue or connect.

> **“A name is just a label — real truth lives in the signal and the moment it’s captured.”**
