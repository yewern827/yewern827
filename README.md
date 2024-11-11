#Procedure
def jadual():
    ulangan="YA"
    while ulangan=="YA":
        print("Kasut putih:RM45,kadar diskaun:10%")
        print("Beg sekolah:RM50,kadar diskaun:20%")
        print("Pen biru:RM1.60,kadar diskaun:0%")
        print("Buku teks:RM20,kadar diskaun:5%")
        kasutputih = int(input("Sila masukkan kuantiti Kasut putih:"))
        begsekolah = int(input("Sila masukkan kuantiti Beg sekolah:"))
        penbiru = int(input("Sila masukkan kuantiti Pen biru:"))
        bukuteks = int(input("Sila masukkan kuantiti Buku teks:"))
        print ("RM",kira(kasutputih,begsekolah,penbiru,bukuteks))
        ulangan = input("Adakah anda mempunyai item lain yang ingin dibeli (YA/TIDAK):")
        if ulangan=="TIDAK":
            print("Terima kasih")
           
def kira(kasutputih,begsekolah,penbiru,bukuteks):
    hargakasutputih = (45*0.9)*kasutputih
    hargabegsekolah = (50*0.8)*begsekolah
    hargapenbiru = (1.6*1)*penbiru
    hargabukuteks = (20*0.95)*bukuteks
    jumlahharga = hargakasutputih+hargbegsekolah+hargapenbiru+hargabukuteks
    return jumlahharga
jadual()
