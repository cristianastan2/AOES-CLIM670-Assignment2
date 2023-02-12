---
title: "Assignment #2"
teaching: 0
exercises: 0
questions:
- "What do I need to do for Assignment #2"
objectives:
---

### What is expected?

1. The physics suites and primary schemes supported in CCPP v6.0.0 are listed in Table 1 adapted from [DTC](https://dtcenter.ucar.edu/GMTB/v6.0.0/sci_doc/allscheme_page.html).

Table 1

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

2. 

3. 


### When is it due?
Feb 27

### How do I turn it in?
Email me your essay.
