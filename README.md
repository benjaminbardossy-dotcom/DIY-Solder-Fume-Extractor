# Cheap DIY Solder Fume Extractor


# Why Make Your Own? / Why I Made This
Many of the cheap solder fume extractors sold online don't effectively remove the harmful particles created from soldering, and only feature an activiated carbon filter. Activated carbon is great at removing the smell associated with soldering, but falls flat when filtering out the smaller harmful particles. Theres also no guarantee of the strength of the fan, or lifetime of the filter. Once either of those die theres no telling how easy or hard it will be to replace.
### But why is that?
Activated carbon mainly removes volatile organic compounds(VOCs), which are responsable for the smell associated with soldering. However, activated carbon is not nearly as effective at trapping other small particles created from soldering, since it cannot reliably catch them.
### My Solution
Create your own! Creating a good fume extractor shouldn't be hard or expensive, which is why I made this project easily replicable for the average hobbyist.

If you want a full cost breakdown, check out the spreadsheet I made for this project [here](https://docs.google.com/spreadsheets/d/1kI0-QvfijKjpn8jp-Lh3tqiNpf6TtSSo3WHpc60xSvA/edit?gid=0#gid=0)
# The Design

## The filter
For my fume extractor, I decided to add a multi stage filtration system. The media goes as follows: Pre-Filter -> HEPA -> Activated Carbon. The pre-filter acts as a barrier to catch large particles which may stick to and clog the finer filter media such as the HEPA filter. This extends the lifetime of both the fan and other filter media. The HEPA filter serves as the solution to trapping finer particles. It effectively filters out 99.97% of particles with a size of 0.3 microns([source](https://www.epa.gov/indoor-air-quality-iaq/what-hepa-filter)), and even filters out smaller particles(0.3 microns is just the benchmark for measuring effectiveness). I still included an activated carbon layer, since it is still best to also remove any remaining VOCs.

## The Case
<img width="802" height="719" alt="image" src="https://github.com/user-attachments/assets/35c947b6-7a79-48b8-b657-3b1425ff4c3d" />\
Before creating my case, I thought of what I wanted in a fume extractor. I wanted an easily printed case with internals made from components readily available to the average hobbyist, and I wanted it to be cheaper than the extractors available online. To do so I created a case which prints in seperate parts and is attached by M2 inserts and screws, a top which screws off to reveal both the filter media and pc fan, and an open source design which can be easily modified to fit any hobbyists components. As for the price, I managed to keep it at a cost of just under $22 CAD for one build.

# Creating Your Own
This design was made to be easily replicable for the average hobbyist, and if your interested in creating your own, I created this guide to help at every step.

1. Gather the Necessary Files(All files / folders referenced can be found at the top of this repo)
   - Download the STL files found in folder Fume Extractor STLs
3. Gather the Materials
   - Order any missing components from the BOM list below
   - Upload the STL files to a 3D printing software of your choice and print the case, OR alternatively order the STL files to a vender which offers 3D printing services if you don't have access to a 3D printer
4. Assemble
   - Gather your parts needed
   - Use a solder pen with the M2 insert attachment to heat up the inserts and place them into their designated spots on the model(see design photos)
   - Superglue the switch into place in its designated spot
   - Cut the head off of the 12V adapter to expose the positive and negative wires
   - Solder the positive wire to one end of the switch, and the negative to the other
   - Strip the ends of the positive and negative wires of the fan
   - Solder the positive wire to the switch where the positive wire of the 12V adapter is wired, do the same for the negative terminal
   - Place objects as shown in the design photo
   - Use M2 nuts to secure fan
   - Use M2 screws to screw the case into place
   - Place filter media as shown: Pre-filter -> HEPA filter -> Activated carbon filter
   - Screw top on

# BOM
| Material      | Quantity      | Cost($CAD)     | Link          |
| ------------- | ------------- | ------------- | ------------- |
| M2 Screws| 12 | 0.26 | https://www.amazon.ca/780Pcs-Screws-Metric-Washers-Steel-Black/dp/B0D7QCS5FL?source=ps-sl-shoppingads-lpcontext&ref_=fplfs&smid=A3GSZ4RKHEJUDQ&th=1 |
| M2 Nuts | 4 | 0.09 | https://www.amazon.ca/780Pcs-Screws-Metric-Washers-Steel-Black/dp/B0D7QCS5FL?source=ps-sl-shoppingads-lpcontext&ref_=fplfs&smid=A3GSZ4RKHEJUDQ&th=1 |
| M2 Heat Inserts | 8 | 1.12 | https://www.amazon.ca/HANGLIFE-Heat-Set-Threaded-Components-Soldering/dp/B0D477R64K?th=1 |
| PC Fan | 1 | 6.53 | https://www.aliexpress.com/item/1005002971846100.html?spm=a2g0o.productlist.main.27.341eL2suL2suXO&utparam-url=scene%3Asearch%7Cquery_from%3Apc_back_same_best%7Cx_object_id%3A1005002971846100%7C_p_origin_prod%3A&algo_pvid=ec0875f1-128a-41e3-a1c4-d19c2a85521f&algo_exp_id=ec0875f1-128a-41e3-a1c4-d19c2a85521f&pdp_ext_f=%7B%22order%22%3A%223117%22%2C%22fromPage%22%3A%22search%22%7D&pdp_npi=6%40dis%21CAD%215.83%215.59%21%21%214.16%213.99%21%402101c44517787165821202264ece57%2112000036189434570%21sea%21CA%216516785883%21X%211%210%21n_tag%3A-29919%3Bd%3Ab1c396d5%3Bm03_new_user%3A-29895 |
| Prefilter | 38.40cm^3 | 0.05 | https://www.aliexpress.com/item/1005005513088209.html?spm=a2g0o.detail.0.0.7624pQ4EpQ4E9v&mp=1&pdp_npi=6%40dis%21CAD%21CAD+9.58%21CAD+9.58%21%21CAD+9.25%21%21%21%402101d9ef17787169355696266eed95%2112000033368451967%21ct%21CA%216516785883%21%211%210%21 |
| HEPA Filter | 2 | 2.52 | https://www.aliexpress.com/item/1005002687133564.html?spm=a2g0o.detail.0.0.711cRoQARoQArh&mp=1&pdp_npi=6%40dis%21CAD%21CAD+7.55%21CAD+7.55%21%21CAD+7.20%21%21%21%40210325a917787084133755726e8646%2112000044392096372%21ct%21CA%216516785883%21%211%210%21&pdp_ext_f=%7B%22cart2PdpParams%22%3A%7B%22pdpBusinessMode%22%3A%22retail%22%7D%7D |
| Activated Carbon Filter | 32.00cm^3 | 0.003 | https://www.aliexpress.com/item/32789944517.html?spm=a2g0o.productlist.main.1.1eea583c2ZqgGh&algo_pvid=e94bd99e-fb68-4f1f-b958-793e0c4c6bb3&algo_exp_id=e94bd99e-fb68-4f1f-b958-793e0c4c6bb3-0&pdp_ext_f=%7B%22order%22%3A%221543%22%2C%22eval%22%3A%221%22%2C%22fromPage%22%3A%22search%22%7D&pdp_npi=6%40dis%21CAD%213.78%213.70%21%21%212.70%212.64%21%40210328c017787068095315435ee6af%2112000017994405074%21sea%21CA%216516785883%21X%211%210%21n_tag%3A-29919%3Bd%3Ab1c396d5%3Bm03_new_user%3A-29895&curPageLogUid=XRfYtDNrAWy3&utparam-url=scene%3Asearch%7Cquery_from%3A%7Cx_object_id%3A32789944517%7C_p_origin_prod%3A|
| Potentiometer | 1 | 0.98 | https://www.aliexpress.com/item/1005006143559414.html?spm=a2g0o.order_list.order_list_main.80.261d1802WHEldB |
| Electronic Switch | 1 | 0.68 | https://www.aliexpress.com/item/1005008778176373.html?spm=a2g0o.productlist.seoads.5.43af3f86OP2rfn&p4p_pvid=20260512143655131318433995970003058183_3 |
| 12V 1A Adapter | 1 | 6.01 | https://www.aliexpress.com/item/1005001731366424.html?src=google&src=google&albch=shopping&acnt=631-313-3945&isdl=y&slnk=&plac=&mtctp=&albbt=Google_7_shopping&aff_platform=google&aff_short_key=UneMJZVf&gclsrc=aw.ds&albagn=888888&ds_e_adid=&ds_e_matchtype=&ds_e_device=c&ds_e_network=x&ds_e_product_group_id=&ds_e_product_id=en1005001731366424&ds_e_product_merchant_id=108704417&ds_e_product_country=CA&ds_e_product_language=en&ds_e_product_channel=online&ds_e_product_store_id=&ds_url_v=2&albcp=19366866438&albag=&isSmbAutoCall=false&needSmbHouyi=false&gad_source=1&gad_campaignid=17337458112&gbraid=0AAAAACbpRIlN7eGJpvL5wv0rmG_zhkeAF&gclid=CjwKCAjwtvvPBhBuEiwAPMijr9Ke-8rEegY7HdN6hDKmidVHpZvyaxiaOKmjk-yy1-_iUfwRmOnaAhoCOAkQAvD_BwE |
| 3D Printer Filament | 84.37g | 1.69 | https://www.amazon.ca/ELEGOO-Filament-Dimensional-Accuracy-Printers/dp/B0D421Q2Q2/ref=asc_df_B0D421Q2Q2?mcid=26a2768281f1302498f5d97790c34073&tag=googleshopc0c-20&linkCode=df0&hvadid=706827341264&hvpos=&hvnetw=g&hvrand=17333765710625862393&hvpone=&hvptwo=&hvqmt=&hvdev=c&hvdvcmdl=&hvlocint=&hvlocphy=9000685&hvtargid=pla-2350142291737&hvocijid=17333765710625862393-B0D421Q2Q2-&hvexpln=0&gad_source=1&th=1 |
| Heat Shrink | 2 | 0.80 | https://www.aliexpress.com/item/1005008895688869.html?spm=a2g0o.productlist.main.2.5d6c4adekYd0k0&algo_pvid=731cefd1-6197-4baf-ac3e-f355999f682c&algo_exp_id=731cefd1-6197-4baf-ac3e-f355999f682c-1&pdp_ext_f=%7B%22order%22%3A%2210450%22%2C%22spu_best_type%22%3A%22price%22%2C%22eval%22%3A%221%22%2C%22fromPage%22%3A%22search%22%7D&pdp_npi=6%40dis%21CAD%214.86%214.79%21%21%2123.60%2123.25%21%402103128917786209916383607e4708%2112000047111301585%21sea%21CA%216516785883%21X%211%210%21n_tag%3A-29919%3Bd%3Ab1c396d5%3Bm03_new_user%3A-29895&curPageLogUid=DUcnDSfQfAhJ&utparam-url=scene%3Asearch%7Cquery_from%3A%7Cx_object_id%3A1005008895688869%7C_p_origin_prod%3A |
