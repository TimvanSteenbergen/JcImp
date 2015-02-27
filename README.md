This is the code for the MyShop-shops for company JcImp.
Customer is JcImp, a company selling cosmetic products to other shops. Each other shop gets their own version of the shop.

Versioncontrol in Git: https://github.com/busymachines/myshop;
Ticketcontrol in Jira; https://tiekanearshore.atlassian.net/secure/Dashboard.jspa
Documents on GoogleDrive: http://docs.busyweb.nl -> Customer JcImp

Sequence of work for making changes to JcImp's shops;
- Releasemanager creates a Jira-ticket and assigns it to a programmer
- Programmer creates a new branch shopx-y-shortdescription from master-branch (when y is last-version-plus-1)
- Programmer makes the changes, and via MyShop-editor uploads all necessary files to the shop 43375xx.myshop.nl
- Programmer pushes the changes to branch issuexyz-shortdescription
- Programmer creates a pull request and changes the status of the Jira-ticket, putting the url of that pull-request in a comment.
- Testers (Releasemanager and customer(s)) check the changes and if something needs to change, inform the programmer;
- Programmer can change it into the same branch and when it’s ready again report via Jira to testers.
- Testers check the changes and if it is ok, Releasemanager merges it into the master branch.
     From then on the branch issuexyz-shortdescription is not to be used anymore, it’s just there for history.

Shop's codeparts in the myshop-editor:
- skin.html and base.css (and theme.css if used). Upload them in the editor to
    Pages->Home page->Button 'Skin'->Menu 'Eigen layout'
- productlist.html. Upload it in the editor to
    Products->Product list 1 (Consumenten)->Button 'Own layout'
- (@TODO: check if this is still functioning) productlist.css. Upload it in the editor
    first go to shopnr 00, then go to Pages->Pictures and other documents->'other pictures and files'
- images. Upload them in the editor
    first go to shopnr 00, then go to Pages->Pictures and other documents->'other pictures and files'

These are the customers of JcImp:
    Shopnr  Customer                url                                                   Customersite
    01      Shopschsp               http://shopschsp.jc-imp.nl/                           www.jc-imp.nl
    02      Dermaclinic             http://dermaclinicshop.jc-imp.nl/                     ..
    03                              http://kvegshop.jc-imp.nl/
    04      cspshop                 http://cspshop.jc-imp.nl/
    05      cspshop                 http://cspshop.jc-imp.nl/
    06                              http://ompzoshnonmed.jc-imp.nl/
    07      Van Brakel              http://vbrakelshop.jc-imp.nl/
    08      HaShop                  http://hashop.jc-imp.nl/
    09      Beautifulshop           http://beautifulshop.jc-imp.nl/
    10      van Eunen               http://vaneunenshop.jc-imp.nl/
    11      Huidzorg Houten         http://huidzorghouten.jc-imp.nl/
    12      Tamara Totaal           http://tamaratotaal.jc-imp.nl/
    13      Beautycorner            http://beautycorner.jc-imp.nl/
    14      testshop
    15      testshop
    16      testshop
    17      testshop
    18      testshop
    19      van Lennep              http://vanlennepshop.jc-imp.nl/
    20      Annelies                http://medispaannelies.jc-imp.nl/
    21      GC Aesthetics           http://gcavipstore.colorescience.nl/gc-aesthetics
    22      Derma2Care              http://derma2care.jc-imp.nl
    23      Villa Vital             http://villavital.jc-imp.nl/
    24      Mooi medisch Sportief   http://mooimedischsportief.jc-imp.nl/
    25      Stendershop             http://stendershop.jc-imp.nl/                       www.annettestender.nl
    26      Beauty Results          http://260326.mijnwinkel.nl/                        www.beautyresult.nl


