Data from Wheeler & Kipping 201?.  Find our code at [github.com/ajwheeler/sebastien](github.com/ajwheeler/sebastien)

- `detections.csv` contains the period with the highest zeta value (merit function) for each KIC we analyzed.  The `is_known` column is true for KICs we threw out in our analysis , i.e. those in the Villanova eclipsing binary catalog (Kirk et al. 2016; Abdul-Masih et al. 2016), Kepler KOIs and TCEs (Thompson et al. 2018), the candidates from (Huang et al. 2013), the long-period candidates from the wavelet-based search of Foreman-Mackey et al. (2016) and planet hunters (Wang et al. 2015), and the ultra-short period planets in Sanchis Ojeda et al. (2015)

- `multinest_files` contains the output of `multinest` for each fit to a transit candidate (each row in table 2).

  * the parameters for the candidates fit with e==0 (KIC 4754691, KIC 9955874, and KIC 10190048) are `["$t_0$", "$R_p/R_*$","$\\log(P)$", "$b$", "$\\log(\\rho_*)$", "$q_1$", "$q_2$", "A", "B"]`, where `A` and `B` specify a local linear trend of the form `A*(t-t0) + B`

  * the parameters for the candidates fit with eccentricity unfixed (KIC 5475628 and KIC 10474113) are `["$cos(w)$", "$sqrt(e)sin(w)$", "$t_0$", "$R_p/R_*$","$\\log(P)$", "$b$", "$\\log(\\rho_*)$", "$q_1$", "$q_2$", "A", "B"]`, where `A` and `B` specify a local linear trend of the form `A*(t-t0) + B`

  * the parameters for KIC 7947784 are ` ["$t_1$", "$R_1/R_*$", "$\log(P_1)$", "$b_1$", "$A_1$", "$B_1$", "$t_2$", "$R_2/R_*$","$\log(P_2)$", "$b_2$", "$A_2$", "$B_2$", "$\\log(\\rho_*)$", "$q_1$", "$q_2$"]`

  * the parameters for KIC 8508736 are `["$t_1$", "$t_2$", "$R_p$", "$a$", "$b$", "$q_1$", "$q_2$"]`
