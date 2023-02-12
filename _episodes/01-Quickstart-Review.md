---
title: "Assignment #2"
teaching: 0
exercises: 0
questions:
- "What do I need to do for Assignment #2"
objectives:
---

### What is expected?

1. Select two SCM cases designed to simulate ocean (land) environmental conditions.
2. Select two physics suites that are relevant for the representation of precipitation in the selecsted environment. 
3. Conduct simulations for each possible combination of cases and suites (4 experiments). Th elength of the experiment should not exceed 4 days.
4. Compare the time series of precipitation (mm/day) for all experiments. 
5. For a period with active/suppressed precipitation compare the vertical profiles of each tendency term of specific humidity (q, units: g kg<sup>-1</sup>/day) and temperature (units: K/day) for all experiments.
6. Discuss similarities and differences you observee when analyzing your simulations. 

**The physics suites and primary schemes supported in CCPP v6.0.0** are listed in the table below adapted from [DTC](https://dtcenter.ucar.edu/GMTB/v6.0.0/sci_doc/allscheme_page.html).

| **Physics Suites**  | **GFS_v16** | **GFS_v17_p8** | **RAP** | **HRRR** | **RRFS_v1beta** | **WoFS_V0** |
| --- | --- | --- | --- | --- | --- | --- |
| **Deep Cu** | [GFS Scale-Aware Simplified Arakawa Schubert (sa-SAS) Deep Convection Scheme](https://dtcenter.ucar.edu/GMTB/v6.0.0/sci_doc/_g_f_s__s_a_m_fdeep.html) | [GFS Scale-Aware Simplified Arakawa-Schubert (sa-SAS) Deep Convection Scheme + Cellular Automata Stochastic Convective Organization Scheme](https://dtcenter.ucar.edu/GMTB/v6.0.0/sci_doc/_g_f_s__s_a_m_fdeep.html#ca_page) | [Grell-Freitas Scale and Aerosol Aware Convection Scheme](https://dtcenter.ucar.edu/GMTB/v6.0.0/sci_doc/_c_u__g_f.html) | off | off | off |
| **Shallow Cu** | [GFS SAS-based Mass-Flux Scheme for Shallow convection (sa-MF)](https://dtcenter.ucar.edu/GMTB/v6.0.0/sci_doc/_g_f_s__s_a_m_fshal.html) | [GFS SAS-based Mass-Flux Scheme for Shallow convection (sa-MF)](https://dtcenter.ucar.edu/GMTB/v6.0.0/sci_doc/_g_f_s__s_a_m_fshal.html) | [Grell-Freitas Scale and Aerosol Aware Convection Scheme](https://dtcenter.ucar.edu/GMTB/v6.0.0/sci_doc/_c_u__g_f.html) | [MYNN-EDMF Boundary Layer and Shallow Cloud Scheme](https://dtcenter.ucar.edu/GMTB/v6.0.0/sci_doc/_m_y_n_n_e_d_m_f.html) | [MYNN-EDMF Boundary Layer and Shallow Cloud Scheme](https://dtcenter.ucar.edu/GMTB/v6.0.0/sci_doc/_m_y_n_n_e_d_m_f.html) |[MYNN-EDMF Boundary Layer and Shallow Cloud Scheme](https://dtcenter.ucar.edu/GMTB/v6.0.0/sci_doc/_m_y_n_n_e_d_m_f.html) |
| **Microphysics** | [GFDL Cloud Microphysics Scheme](https://dtcenter.ucar.edu/GMTB/v6.0.0/sci_doc/_g_f_d_l_cloud.html) | [Thompson Aerosol-Aware Cloud Microphysics Scheme](https://dtcenter.ucar.edu/GMTB/v6.0.0/sci_doc/_t_h_o_m_p_s_o_n.html) w/o aerosol-aware | [Thompson Aerosol-Aware Cloud Microphysics Scheme](https://dtcenter.ucar.edu/GMTB/v6.0.0/sci_doc/_t_h_o_m_p_s_o_n.html) | [Thompson Aerosol-Aware Cloud Microphysics Scheme](https://dtcenter.ucar.edu/GMTB/v6.0.0/sci_doc/_t_h_o_m_p_s_o_n.html) | [Thompson Aerosol-Aware Cloud Microphysics Scheme](https://dtcenter.ucar.edu/GMTB/v6.0.0/sci_doc/_t_h_o_m_p_s_o_n.html) | [NSSL 2-moment Cloud Microphysics Scheme](https://dtcenter.ucar.edu/GMTB/v6.0.0/sci_doc/_n_s_s_l_m_i_c_r_o_page.html) |
| **PBL/TURB** | [GFS Scale-aware TKE-based Moist Eddy-Diffusion Mass-Flux (EDMF) PBL and Free Atmospheric Turbulence Scheme](https://dtcenter.ucar.edu/GMTB/v6.0.0/sci_doc/_g_f_s__s_a_t_m_e_d_m_f_v_d_i_f_q.html) | [GFS Scale-aware TKE-based Moist Eddy-Diffusion Mass-Flux (EDMF) PBL and Free Atmospheric Turbulence Scheme](https://dtcenter.ucar.edu/GMTB/v6.0.0/sci_doc/_g_f_s__s_a_t_m_e_d_m_f_v_d_i_f_q.html) | [MYNN-EDMF Boundary Layer and Shallow Cloud Scheme](https://dtcenter.ucar.edu/GMTB/v6.0.0/sci_doc/_m_y_n_n_e_d_m_f.html) | [MYNN-EDMF Boundary Layer and Shallow Cloud Scheme](https://dtcenter.ucar.edu/GMTB/v6.0.0/sci_doc/_m_y_n_n_e_d_m_f.html) | [MYNN-EDMF Boundary Layer and Shallow Cloud Scheme](https://dtcenter.ucar.edu/GMTB/v6.0.0/sci_doc/_m_y_n_n_e_d_m_f.html) | [MYNN-EDMF Boundary Layer and Shallow Cloud Scheme](https://dtcenter.ucar.edu/GMTB/v6.0.0/sci_doc/_m_y_n_n_e_d_m_f.html) |
| **Radiation** | [GFS RRTMG Shortwave/Longwave Radiation Scheme](https://dtcenter.ucar.edu/GMTB/v6.0.0/sci_doc/_g_f_s__r_r_t_m_g.html) | [GFS RRTMG Shortwave/Longwave Radiation Scheme](https://dtcenter.ucar.edu/GMTB/v6.0.0/sci_doc/_g_f_s__r_r_t_m_g.html) | [GFS RRTMG Shortwave/Longwave Radiation Scheme](https://dtcenter.ucar.edu/GMTB/v6.0.0/sci_doc/_g_f_s__r_r_t_m_g.html) | [GFS RRTMG Shortwave/Longwave Radiation Scheme](https://dtcenter.ucar.edu/GMTB/v6.0.0/sci_doc/_g_f_s__r_r_t_m_g.html) | [GFS RRTMG Shortwave/Longwave Radiation Scheme](https://dtcenter.ucar.edu/GMTB/v6.0.0/sci_doc/_g_f_s__r_r_t_m_g.html) | [GFS RRTMG Shortwave/Longwave Radiation Scheme](https://dtcenter.ucar.edu/GMTB/v6.0.0/sci_doc/_g_f_s__r_r_t_m_g.html) |
| **Surface Layer** | [GFS Surface Layer Scheme](https://dtcenter.ucar.edu/GMTB/v6.0.0/sci_doc/_g_f_s__s_f_c_l_y_r.html) | [GFS Surface Layer Scheme](https://dtcenter.ucar.edu/GMTB/v6.0.0/sci_doc/_g_f_s__s_f_c_l_y_r.html) | [MYNN Surface Layer Scheme](https://dtcenter.ucar.edu/GMTB/v6.0.0/sci_doc/_s_f_c__m_y_n_n_s_f_l.html) | [MYNN Surface Layer Scheme](https://dtcenter.ucar.edu/GMTB/v6.0.0/sci_doc/_s_f_c__m_y_n_n_s_f_l.html) | [MYNN Surface Layer Scheme](https://dtcenter.ucar.edu/GMTB/v6.0.0/sci_doc/_s_f_c__m_y_n_n_s_f_l.html) | [MYNN Surface Layer Scheme](https://dtcenter.ucar.edu/GMTB/v6.0.0/sci_doc/_s_f_c__m_y_n_n_s_f_l.html)
| **LSM** | [GFS Noah Land Surface Model](https://dtcenter.ucar.edu/GMTB/v6.0.0/sci_doc/_g_f_s__n_o_a_h.html) | [GFS NoahMP Land Surface Model](https://dtcenter.ucar.edu/GMTB/v6.0.0/sci_doc/_noah_m_p.html) | [RUC Land Surface Model](https://dtcenter.ucar.edu/GMTB/v6.0.0/sci_doc/_r_u_c_l_s_m.html) | [RUC Land Surface Model](https://dtcenter.ucar.edu/GMTB/v6.0.0/sci_doc/_r_u_c_l_s_m.html) | [GFS NoahMP Land Surface Model](https://dtcenter.ucar.edu/GMTB/v6.0.0/sci_doc/_noah_m_p.html) | [GFS Noah Land Surface Model](https://dtcenter.ucar.edu/GMTB/v6.0.0/sci_doc/_g_f_s__n_o_a_h.html) |
| **Gravity Wave Drag** | [Unified Gravity Wave Physics Scheme - Version 0](https://dtcenter.ucar.edu/GMTB/v6.0.0/sci_doc/_g_f_s__u_g_w_p_v0.html) | [GFS Unified UGWP Scheme](https://dtcenter.ucar.edu/GMTB/v6.0.0/sci_doc/_g_f_s__u_n_i_f_i_e_d__u_g_w_p.html) | [GSL Drag Suite Scheme](https://dtcenter.ucar.edu/GMTB/v6.0.0/sci_doc/_g_f_s_drag_suite.html) | [GSL Drag Suite Scheme](https://dtcenter.ucar.edu/GMTB/v6.0.0/sci_doc/_g_f_s_drag_suite.html) | [Unified Gravity Wave Physics Scheme - Version 0](https://dtcenter.ucar.edu/GMTB/v6.0.0/sci_doc/_g_f_s__u_g_w_p_v0.html) | [Unified Gravity Wave Physics Scheme - Version 0](https://dtcenter.ucar.edu/GMTB/v6.0.0/sci_doc/_g_f_s__u_g_w_p_v0.html) |
| **Sea Ice** | [GFS Sea Ice Scheme](https://dtcenter.ucar.edu/GMTB/v6.0.0/sci_doc/_g_f_s__s_f_c_s_i_c_e.html) | [GFS Sea Ice Scheme](https://dtcenter.ucar.edu/GMTB/v6.0.0/sci_doc/_g_f_s__s_f_c_s_i_c_e.html) | [RUC Land Surface Model](https://dtcenter.ucar.edu/GMTB/v6.0.0/sci_doc/_r_u_c_l_s_m.html) | [RUC Land Surface Model](https://dtcenter.ucar.edu/GMTB/v6.0.0/sci_doc/_r_u_c_l_s_m.html) | [GFS Sea Ice Scheme](https://dtcenter.ucar.edu/GMTB/v6.0.0/sci_doc/_g_f_s__s_f_c_s_i_c_e.html) | [GFS Sea Ice Scheme](https://dtcenter.ucar.edu/GMTB/v6.0.0/sci_doc/_g_f_s__s_f_c_s_i_c_e.html) |
|  |  |  |  |  |  |  |

**Observations available** to drive the SCM are:

![Tropical Warm Pool - International Cloud Experiment](/fig/TWP-ICE.png)

![Atmosphere Radiation Measurement Southern Great Plains](/fig/ARM-SGP.png)

![Atlantic Stratocumulus to Cumulus Transition Experiment](/fig/ASTEX.png)

![LES ARM Symbiotic Simulation and Observation](/fig/LASSO.png)

![Barbados Oceanographic and Meteorological EXperiment](/fig/BOMEX.png)



### When is it due?
Feb 27

### How do I turn it in?
Upload your homework to Blackboard.
