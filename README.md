# AdvancedHuntingQueries
My collection of Microsoft 365 Advanced Hunting Queries written in Kusto Query Language (KQL). Clicking on the name of the query will bring you to the file for it in this git repo.

***Or try them out right away in your M365 Security tenant:***

Click on the '🔎' hotlink to plug the query right into your Advanced Hunting Query page

## Queries:

### [🔎](https://security.microsoft.com/hunting?query=H4sIAAAAAAAEAI1Vy27TQBS9ayT-YdSVIwXCQ6xQNkCLWAAS7a5CkWM7iandWLaTtIiP59wzM_akmUhdJPO473PPHc9kJka-SiE91l422Om6lQbrB_xy3OyllAxrh_MBOlvsVG8pKe0KecAvkx1OJaT31NxAuqee7vLAf00PaplCd4tzKhXWHe1K3GXSQjNlnJfyAlKbocp67Ft4Vhsjc_zeyjt4_nik-Ym5XTIDtemc7pegnlCqtv9cfQWja7SO-WnEGoj08ijJkYcfiFJjnUTtr6BVBVqG0XJ4PUCiaBi5kNcOxwtXwWnm3rfidIfbV8SlhQ_bE2vxmQjes3qtNBvOCfIz7IuRG1jVtOuZlfZ5BV_aBe3HGrtE3ssb5DlxXDBE4eD8dMSjiXZjCYRMFCFfg3KldzgYeFzBTqNO6VlzVuymjl1aZ8U4BWPPqTXWviA_M2bfOF4ujlhl9ZITjCYBqnsgqnk1tMzZRdufBVftfkmJatksrlze34J7X4tHTfnSQLaFJHFoaRUzTt1lENHWuxumsGRfe9crPxMVNHI3oZvh3kcv2V8vSYFRi_9H7rtoxjHOjjXM3WyZIeOfzKJwPEkZcUob5bllguVZxbgWhQ5VluRtd4YF14PG9cAAi7J6yNmzJScpCThyG6nod4DvzYDjgfkpP9dPXrqO_ckgX5GvIQctbh1OKk-Zb8iN0UtOr-rH64w1-4o71FCTk8rdv7T7jtPDSc01b5MoKpNnzVj4flvt00g5-5ENNn8gsQy6c6yaM9M1auw5VzoD8XfVviyxjHwvfmE_Rgjzi30Bnn5zLI9S10OLekmunX8rY3g_7508j6-dUq0hibyj08iLOL4yrWO7nRE_2Rm_jS3O_wFeOI2figcAAA&runQuery=true&timeRangeId=week) [AnomalousBatExecTimeline](Anomalies/AnomalousBatExecTimeline.kusto)
- Gets the top 5 devices that have had an anomalous spike in execution of .bat scripts

### [🔎](https://security.microsoft.com/hunting?query=H4sIAAAAAAAEAI1Vy47TQBDsMxL_4KMjBS0PcUI5ILSglUBIZDkhFHltbzLETqw4jw3i46munrFndwe0B79m-lFdXT2-kAvJ5JPUssdzLyu86XMrHZ5vcR2kx9oO90xO2N_yO5MGb0tcG-6spJAj1_WtimK19NDoBWy3-C7oe6Cfw1qJ6DVWNe5zeQZEimnOrEdYlIxT4FnSb4No6tsTzYkxlkTaMX_NeOphzxqWHe4lLDV3I2d6H7jufNSeuRvPhGMWQ6A-mcxwvZLXiP-OlleosqaVw3WWzwMfl2TCUKrlH89cwOWwrkxo_BYI1DuX9_fq-471jUwGf2VtDfsXvhuOVWVR1g-Dr2EdY-WIk9Emk2t4tvTdI2JLxm4RT_uijGmsXN7IS1Q38UrIiPbk4_TE3SU5uiGzqUpCHbXc0WdDjeTI3TDrlJHVSzmaMpYpomGemrlntBrrX7AHJdF3XpmLezozuzzJU8zuEcwqto7eFTvmqOEFn9opxx21MiQfPfaraD3UE5jT3qr2ttjJPWNaiWn8MspoNR-GOXTs7973K0xKA4vKz-hqWA_ZHXscdlT_O9zPfO-TiFP6HGuYedVnA-KvRFF7rRTMOKWPg5epwbRmU2Ys2Jyt2Yu0EuaDxXxQgbGsESr27IbTmUc6-ZGo6GfE7_XA44n4VKPLB2fdeDbc8iyIdWi89fiys0PxxtoYo1SMqnGCzVhzqFhPnJa6VP3-pt8XfN09qrnlap5kZfKkOYtPcLN-nKliP8rB5xd2TEFrr6oZkS5R456zpTOQPfHkCydOCmXozzdYj1ljzKl_xYG-_aCqwnfUeuCovPiv9D_en35u_ptrm1jFnifO1WnihBxPnJ1Xvs1LmPKSf88dvv8CF8PqqJgHAAA&runQuery=true&timeRangeId=week) [AnomalousLogonTimeline](Anomalies/AnomalousLogonTimeline.kusto)
- Gets the top 5 users whose logons had the most anomalous spike and projects their daily logins onto a timechart for visual aid
- Service accounts showing up in this query are especially suspicious

### [🔎](https://security.microsoft.com/v2/advanced-hunting?query=H4sIAAAAAAAEAJ1TyUoDQRCts-A_DIPnDOhN8CAYUHA5eZZ20pm0s3SYHg2CH--r151JjIFoGNJdXcurV0sKKSSTW3mXTgZIc_HS417iHsRS68RIQ90CcuDZSQWNlRY2B2vAa4DFEKWhR02dx2nwe4CuBLaHr0ce9XuSa2TWOI3xwNS4UzkBq2LHrkg1GWmuEpgd7gqIJnFXP4v7AroZ-RpIg3xStpBb8g84fcJZQdY4zzwZdFq1SRVUzNRDM_vRi7DF8X7kHXtgyFIzNpBLyp5cNxVOmLcDqocU8O7gN9Cz3_Fsf_VN0SI_C3uJd8tKFvTUXjlyaWAPlAKqC2CkdsdaYwXTcX7PyNDIHTDnnFhG-1fCtexBlrwy5uxY67ruHF4DviVel-zM4WqLxL0lWoHTpGmfA2_di2Nz_q1vRcLVDrWsM-xh8t9exI1xvEvYXoDW452PSG-IctyKzQym8pG2LHACcWvOOEflP5FH9m3FztT4R8X5GtRsMTvd-St8GqPZKvbncNS-6jasbrbqcIlTzJJzX165TzrdXL4BRhV_BE4EAAA&runQuery=true&timeRangeId=week) [EmailsWithOAuthRequests](Phishing/EmailsWithOAuthRequests.kusto)
- Hunt for potential phishing emails that link to a Microsoft OAuth login
- OAuth tokens can grant the 3rd party permissions without stealing credentials
- Logins take place on login.windows.net or login.microsoftonline.com which is less suspicious

### [🔎](https://security.microsoft.com/v2/advanced-hunting?query=H4sIAAAAAAAEANVWTU_CQBCds4n_oXjSg3DwZuJJNOEgMY16NbD9oIG22C1fxvjbffNagghEBKoxZLfdmTfzZmenszSkIY48SE8isXgL8ByIjzcjqSSSSweShLoLjBcZQZtB5kN2LEccDXpp0-JcutCnMoFekQ4shvCZwpNHXyFkHlbq28GcYr4DNuTaEDsCwoEH1WaQh9ArUxPPMbwYPNsYOXgU0ZcbyH1GXMT1BvsJ9qUx6H5czDGwOZ6PkA3W7vEEmCKSOmQp1g7972Kv2jrkr5Cui6gFXQTriLkoMnPP3Blm18pteRptIGLa1OSdLAZ-FKnSOsYUo2Bxyl8H_rw9WbQaNNYA6GmFPBaSAEPrqjqWFHXos5qq44jouaj3rNKzifkVKNZiBKxLj9_JX3Aa7Lk63uWO8lyu-1xVuVv7CzntsiLHKxyLvuqWPTGhnZUZ3kzZOVP2oVPqJ-i9RUfS79ZjNzS0icEw4NlF7K2WsRvGOmbkMznbs7_ukoOrMgfZpx1uzoKyF5bellnRWy3E_N_yUvs2Lz9neSLWcqcJ8drVr3mHDFnJszUn04O3HHorlzyH5Yg0A-GXb2J-X-4aUYu5VE3C09muag4bw5yzSZThvTSkB0UtInA_1V1Qcm7-_3LYGAuMByat19XsuEvZ-QDY41I96AkAAA&runQuery=true&timeRangeId=week) [Exfiltration](Hunting/Exfiltration.kusto)
- Non-browser uploading data to Mega cloud storage
- Rclone sync tool (low-confidence malicious activity)
- Renamed Rclone sync tool (high-confidence malicious activity)

### [🔎](https://security.microsoft.com/v2/advanced-hunting?query=H4sIAAAAAAAEAIWSS0vDUBCFz1rwP4S6UTB2L7goVaFQHwsXbtM02EheeJOoIP52vztpJNGWMrR37syZM3PmZqqpAm2Uao0lKrg9a4kFqhTpU5lKzjX3RB_8YjWqwZeGPZVTS2zD3REPfvEO_4aKmJpMF5rBV-GlRKIBQ4sXcc71oDud6VhHzOSneqOy65yD9bfAKv28NVbR49KwL3DURBut6BSDzomWIHyfFv_atNU6MR7PV3OGzJdh4R-toSH8Pvw0vra1uRMUtVsmZ7kvpnmnc7Kd7xZchncPT26RK33zP7Ht9bvoNjnZybCAPbW5uy0VqHskV1q1w_b3GL_F_z6V8bzaK_o9PsGUG2ttXJXOiQ719j18fEbE77Yx_cPMeL657T8nX7DDpWnocIe17a8d4xZke1XOvg6vZ8Ub7lL1A3NOUNvmAgAA&runQuery=true&timeRangeId=week) [HiddenXLLPayload](Hunting/HiddenXLLPayload.kusto)
- Excel spawned by svchost.exe
- Used to bypass ASR rules and deliver payload through COM
- Implementation and writeup can be found at [optiv/Dent](https://github.com/optiv/Dent#remote-xll-payload-mode)

### [🔎](https://security.microsoft.com/v2/advanced-hunting?query=H4sIAAAAAAAAA6VWTW-bQBCdc6X-B9STkZJGrdRLqxzcJmlcRXFVHPVQVZWDsUOEDQLslCo_Pm_eLhhsTOxGaNlhvnf2zdgnciKOnMu1jPD-AXoA-kKGoIagHLkRj5IedtfKR5SP5BISRz7jfQXOT9BXkHuQePJaXsG3el9IgGciGei5hPgOsS-xHIllivc7rAD8XFIpQIekYysxOrncQceRD1gRNDJwslqUAnpL7L6MYe1AeywrWmisCNqhJNiVk-Cd1vw4tJlgX-I74HeEZzOagxVW_sY8WUybCPE1F_Wv_i7BV5sFtObgqe0p1gR6hhci0578kt-o6idI6o85UQbPt3IsD_CVMjvNbQzax-nq0W4oSV8ULZC_0PTpL-NN6C3MOqKew-8YWpH0EWkCDY2c7Rn_0DN6QNbZgSd7-Rn78g8Z6sn6kPm8bcXmfrkcGrWsSQ5-QvR_JKK1NppDBO28gc87i7OshuEQb9NNIVdg--QM1Io5Bsh_ga6KyX_kGQzGNTOTaV372uLqiB0eI_cZO3oI7RJ7WeUrwVcs9-B2e_rCyqY217UfU9WElVHeH_jK4HGB2u6O7lbx54h2DOuE_V50Roo5K3q0LbGyb_6lH5PvrhhvK7pua9D8nKXHu9Tc3IOruzkTTKzc4qXEYK_Sc2mlNf3OXOY2-i47c4J1XvfQCFnNQQN_RYW1strbMdqw_57Yn3K-5LbOU3bC-rdgBumKsRzs2hPLCu2a0wP1Uuq21cn8SmRAmPZOQSRsT263gY7yMZk0p8IQs6y8mYHtRYOv7jnSFWH7Hkuf21O_y8-uad1Wg67J3hWjDT1ltl7jrI92Lua8PdW74K9qVLub02pe-px7Pfla3Xcd6W-4TFcta_Vw_2O6bWahvG843S3-0yiaI8vbVaG2zmvvq6Nn0fME2qq9SJwJAAA&timeRangeId=week) [IdentityCorrelation](Utilities/IdentityCorrelation.kusto)
- Enter any number or combination of the following fields:
    - Hostname
    - Username
    - EmailAddress
    - SID
    - AzureAccountID
- Query will fill in the fields you don't know
- Only needs minimum of 1 value for any 1 field

### [🔎](https://security.microsoft.com/v2/advanced-hunting?query=H4sIAAAAAAAEAI1UW2sTQRQ-z4L_YRqEbGCrPvhaMDQpFRqQtOKDiGyyW7M2m43ZabXij_ebb2b2llkJwy5nzpzLd65zKSSRXLYylyfJZCdaKnkpL-SvKPklG_AO-JTcgTZUAok7eZY96Ar8HDpKIhnLR0jk4G1Ax-CNZQHpLawk1BzLJGh5XmOYyhrWcylp86xlewnJPSQSSBgdg0LztoG2xe293vKegtawpOSnPBJBQilj8xQsM_wNr43oAkfJSD7gtgLvkX5GQUuX1LmHbko8BvcNPpPlLd7XfNf0tmMmR3IN-jtsWItvcJSc8yj5zOxqapss6_rNyHn5PgqfC3O_wlcivinuKd8r-j0LYnkvD6BLWFtB8p28plSBF4VjsWXyGzoFK5M5z12Mx3HMXW2G41F1RCaaClkuWJUD5P7QzxVrY3SaeinWpmAEETo0Z19UjMognLA7btg52YBugniGdS9dxbWTX9f3yEks2S85NPJ6lhrbD-B9q6ONAtLtSWjXaAILK8ycz6bP0yf2Vcn8ZA7ZjlUx1Nb1up8Dw99zClLe7PQYqsmDrb-mlJ80P0s2Kwq27vFPXeWe2FvPLS_e7uEovn7HKnfM_Tjr4YwO5Sh2vWXnq-R-and_v-svetOxcFbDUxJ38N6i7iv54bZD9629J62X8Obsai35XtV7RrkqHphNDV_2LcL8vcIsNrv2i7yVr-Ca-GfQ0p2dtSBnAzplH3W9XtPr_7dDP0-n5GfW6432Xu9KTgN73HsNvTUz6PfDnnh8Lc6JqMTfou1mPw7U7pQsxL0KDc16s7MMAu2mdmjr_AO6LBDpfAcAAA&runQuery=true&timeRangeId=week) [PhishDelivered](Phishing/PhishDelivered.kusto)
- Detects high-confidence phishing or malware emails that were delivered to one or more mailboxes

### [🔎](https://security.microsoft.com/v2/advanced-hunting?query=H4sIAAAAAAAEAO2UX0sCURDFz3PQd9h8qpeEeo4osz9gKa0WQi_iWkmra66lQh--38xusohBFFFBDNe998zMuWfm3mtZZQVq6l59pcxu-cbqMesq0VATdUCG7tthPOoJ7xisB7auNR9lZ2mQMQG3rD55MViYRyfkpawOdA5a1Uwj_Ake22HiEUM8z54ZKOI7JreLLwDpYrZjtucRc4s0rEFcsvBWwTMFWeQL2VOq6zlboM2l-ArzAdYhJ1LNa11dfUk32LWvI7xTUENCzZlZ3QPt0iPDsmzr5V0eY3WXXFGwsAQlwQ_pqbJTS5c64-zbv0pZm9FEn_Vra0lXtvdHlW2s1JYWVIyc5-3Ol1bemOPcewHLIOfdcya7f3YzY_i28cwWHN_zJlJUdfKOZn0fFd7h59_E187ZbN9_T4iu65B6atysOtZ0vKjM1qdwjOGO_D_nQVcwx_TCuhsWaqx4hfN3zuX_Hf-dd_wK0uHsE2YGAAA&runQuery=true&timeRangeId=week) [SeriousSAM](Exploits/SeriousSAM.kusto)
- Hunt for potential exploitation of [SeriousSAM](https://msrc.microsoft.com/update-guide/vulnerability/CVE-2021-36934)
