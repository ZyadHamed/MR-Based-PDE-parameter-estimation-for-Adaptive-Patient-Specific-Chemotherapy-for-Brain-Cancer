# MR-Based-PDE-parameter-estimation-for-Adaptive-Patient-Specific-Chemotherapy-for-Brain-Cancer
Accurately modeling tumor progression and drug interactions in brain cancer
treatment remains challenging. Current approaches lack patient-specific
frameworks that dynamically adapt treatment plans using real-time imaging
feedback and efficiently solve spatiotemporal models for personalized drug
delivery 
# PDE Model

<h3 align="center">Modified PDE Model and Parameter Interpretation</h3>

<table style="border-collapse: collapse; border: none;">
  <tr>
    <td style="border: none;" align="center">
      <span style="font-weight:600;">Model Parameters and Their Biological Interpretation</span><br><br>
      <img src="https://github.com/user-attachments/assets/0da48823-88fe-4e91-972e-3978822e849f" width="400"/>
    </td>

  <td style="border: none;" align="center">
      <span style="font-weight:600;">The Modified Model</span><br><br>
      <img src="https://github.com/user-attachments/assets/62db24c3-067b-41e1-a3a8-98f04c5d8d1d" width="400"/>
    </td>
  </tr>
</table>

# Methodology
- Implemented Brain and Tumor Segmentation
- Implemented PINNs and DeepONet PDE solvers
- Implemented patient-specific diffusivity and initial condition estimation
- Integrated the aforementioned models into one compact system.
<img width="972" height="540" alt="image" src="https://github.com/user-attachments/assets/485eff15-f965-4488-9cf2-79c83f111095" />

# Results

- Deep learning solvers were 59 times faster than the fastest numerical solver. 
- The achieved Dice scores were 0.89 for tumor segmentation and 0.9881 for brain segmentation. 
- The PINN and DeepONet models achieved mean errors of 0.134 and 0.003286.

<img width="2323" height="770" alt="image" src="https://github.com/user-attachments/assets/7dcca1ad-18ee-4b1c-a34b-f64560e3f549" />


# Conclusion

- We developed a 3D PDE-based framework for patient-specific brain cancer treatment planning using MRI segmentation and ADC maps.
- We compared two deep learning models: Physics Informed Neural Network (PINN) and Deep Operator Network (DeepONet).
- Based on results, DeepONet performed better in generalization and solved PDEs at unseen conditions without retraining.
- This approach enables rapid evaluation of treatment scenarios, allowing identification of optimal chemotherapy strategies for adaptive, patient-specific care


# Future Work
- Train DeepONet on more initial conditions to improve accuracy and extend generalization across different diffusivity values.
- Calculate diffusivity from a single MRI image instead of relying on multiple scanning techniques..
- Develop a physical prototype for implementing adaptive treatment plan recommendations in clinical practice.



For more details, check out our full paper attached in the repository!
