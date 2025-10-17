
# SPICE Experiments — Week 4

---
# Contents Learned

## 1. MOSFET Behavior & Id vs. Vds Characteristics
- **Simulate an NMOS device**, sweeping \( V_{ds} \) for different \( V_{gs} \), to observe linear and saturation regions.
- **Plot** \( I_d \) vs. \( V_{ds} \) curves.

## 2. Threshold Voltage Extraction & Velocity Saturation
- **Sweep** \( V_{gs} \) vs. \( I_d \) and extract threshold voltage \( V_t \) (e.g., by linear extrapolation).
- **Observe** effects of velocity saturation in the short-channel regime.

## 3. CMOS Inverter: Voltage Transfer Characteristic (VTC)
- **Build a CMOS inverter** (PMOS + NMOS).
- **Sweep input**, plot \( V_{out} \) vs. \( V_{in} \).
- **Identify** the switching threshold \( V_m \) (the point where \( V_{in} = V_{out} \)).

## 4. Transient Behavior: Rise / Fall Delays
- **Apply a pulse input** to the inverter.
- **Extract rise and fall propagation delays** (times at \( \frac{V_{dd}}{2} \) crossing).

## 5. Noise Margin / Robustness Analysis
- From the VTC plot, determine:
  - \( V_{IL}, V_{IH}, V_{OL}, V_{OH} \)
- Compute:
  - **Noise Margin Low (NML)**: \( NML = V_{IL} - V_{OL} \)
  - **Noise Margin High (NMH)**: \( NMH = V_{OH} - V_{IH} \)

## 6. Power-Supply and Device Variation Studies
- **Vary supply voltage** \( V_{dd} \) and re-plot VTCs to observe how the switching threshold shifts.
- **Modify transistor sizing** (e.g., W/L of PMOS or NMOS) to simulate device variation and observe effects on VTC, noise margins, and delays.

---

# LABS

## 1. day1_nfet_idvds_L2_W5.spice
<img width="1559" height="692" alt="Screenshot From 2025-10-17 11-55-07" src="https://github.com/user-attachments/assets/1e175045-faf9-42a7-9dd9-9adf21e1501e" />


## 2. day2_nfet_idvgs_L015_W039.spice
<img width="1594" height="883" alt="1" src="https://github.com/user-attachments/assets/c3be2f3a-1097-4aa4-af12-92ec1e28db9f" />

## 2(2). day2_nfet_idvds_L015_W039.spice
<img width="1488" height="883" alt="2" src="https://github.com/user-attachments/assets/0cf72e25-7f1b-4222-aa16-b5a7ca0696ca" />

## 3. day3_inv_vtc_Wp084_Wn036.spice
<img width="1488" height="883" alt="3" src="https://github.com/user-attachments/assets/7fd56a83-d628-4b0c-8e4f-7a0673073e19" />

## 3(2). day3_inv_tran_Wp084_Wn036.spice
<img width="1606" height="883" alt="3-2" src="https://github.com/user-attachments/assets/2fc8b12c-77e2-473a-b56c-c016b858a7a9" />

## 4. day4_inv_noisemargin_wp1_wn036.spice
<img width="1586" height="883" alt="4" src="https://github.com/user-attachments/assets/f8b76623-2146-46a7-a946-b24ed6519458" />

## 5. day5_inv_devicevariation_wp7_wn042.spice
<img width="1605" height="883" alt="5-2" src="https://github.com/user-attachments/assets/994b6eb4-f827-42eb-bf3c-8e0574e4a189" />

## 5(2). day5_inv_supplyvariation_Wp1_Wn036.spice
<img width="1602" height="883" alt="5" src="https://github.com/user-attachments/assets/e6ab0641-c402-4132-8f39-2beb7dec0fe9" />
