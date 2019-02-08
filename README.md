# tkinterguidesigner

			Tkinter arayüz yardımcısı hakkında

	Gerekli program ve modüller:Program klasöründe mevcut olanlar dışında:
	** Linux (ubuntu türevleri) ve Python 3.4+
	** Python3-tk (tkinter 8.6)
	** tkarayüz4.py de import bölümündeki modüller kurulu olmalıdır.

	1. Program herhangi bir kurulum gerektirmez. Gönderdiğim "tar" dosyasından çıkartacağınız "arayüz yardımcısı" adlı klasörü Masaüstünüze koyun, "tkarayüz4.py" için çalıştırma yetkisi verin, gerekirse sahibi ve grubunu da değiştirin ve çalıştırın. Klasörü Masaüstü yerine /home dizini altında başka bir konuma da yerleştirebilirsiniz. Program ilk çalıştırıldığında "tkarayüz4.py" dosyasını arar ve yolunu klasör içindeki "anadizyol" dosyasına yazar. Sonraki çalışmalarda bu adrese bakılacağından klasör içindeki dosyaların adlarının değiştirilmesini önermiyorum.
	2. Sistemim Türkçe olduğundan program içinde Türkçe karakterler ve değişken adları da kullanılmıştır. Bu durum, sistemin dili Türkçe değilse sorun çıkarabilir. 
	3. Program çalıştırıldığında küçük bir seçenek penceresi açılacaktır. İlk çalıştırmada "4" seçeneğini seçmeyiniz, çünkü önceden açtığınız bir dosya yok. Kayıt düğmesine basıldığında son açılan dosyanın yolu, "sonyol" adlı dosyaya kaydedilir. Seçenek penceresinde etiketlerin üzerine tıklayarak veya seçenek numarasını yazarak seçim yapabilir, daha sonra Enter tuşuna basarak veya "Tamam" düğmesine tıklayarak programı çalıştırabilirsiniz. Veya "Vazgeç" düğmesine basarak çıkabilirsiniz.
		** Boş form oluştur:Sadece boş bir form açılır. Bu form, kayıt yapıldığında Masaüstüne kaydedilir.
		** Varolan bir dosyayı aç:Mevcut bir form açılır. Bir yeni proje ilk oluşturulduğu zaman, Masaüstünde bir klasör oluşturularak form dosyası ile program dosyası bu klasöre kaydedilir. Siz form dosyasını açıp onun üzerinde işlem yapacaksınız (sonu form ile bitenler). Form üzerinde çalışırken, bu formun çalışma zamanında nasıl görüneceğini ilgili düğmeye basarak anlayabilir, form ve program kodlarını inceleyebilirsiniz.
		** Yeni proje oluştur:Yeni projeye bir isim verin ve ekrandaki talimatları takip edin. Yeni proje klasörü ve içinde program dosyası ile form dosyaları Masaüstünüzde oluşturulur. İsterseniz daha sonra bu klasörün yerini değiştirebilirsiniz.
		** Önceki projeyle devam et: Varsayılan olarak girilmiştir. Doğrudan Enter tuşuna basarak son açılan form dosyasına gidebilirsiniz. Projenin yerini değiştirdiyseniz, aynı dosya ile daha sonraki ilk çalışmada bu seçenek değil, "varolan dosyayı aç" seçeneği seçilmelidir.

	4. Neler yapabilirsiniz?
		* Sol taraftaki Araçlar bölmesinde bulunan araç simgelerine tıklayarak form üzerinde araç oluşturabilirsiniz. Önce forma tıklayın, sonra araç simgesine tıklayın. Her seferinde sadece bir araç oluşturabilirsiniz. Bir araca tıkladığınızda o araç çevresinde kırmızı bir dörtgen belirir (seçim işareti) ve araç özellikleri pencere sol kenarında gösterilir.
Bu alanda araç özelliklerini değiştirebilirsiniz, daha sonra kaydetmeyi unutmayın. Hata durumunda programdan çıkıp tekrar açın.

		*Araç seçmek:Araç ilk oluşturulduğunda özellikleri sol yanda gösterilir. Ayrıca:
					** Araca bir kere sol tıklayarak tek bir araç seçilebilir. Diğer seçimler iptal edilir.
					** Klavyenin solundaki Alt tuşunu basılı tutarak fare hareket ettirilirse, fare okunun üzerinden geçtiği araçlar seçili duruma gelir.
					** Ctrl tuşu basılı tutularak fare sol tıklanırsa birden fazla araç seçilebilir. Seçilen araçların ortak özellikleri sol yanda özellikler penceresinde gösterilir.
					** Seçimi iptal etmek için form üzerinde boş bir alana tıklayın, bütün seçimler iptal edilir.
					** Tek bir seçimi iptal etmek için ctrl+sağ tık birleşimini kullanın.

		* Seçili aracı/araçları hareket ettirebilirsiniz.
			** Aracı seçin, fare sol tuşunu basılı tutarak form üzerinde istediğiniz yere taşıyın ve bırakın.
			** Daha ufak hareketler için aracı seçin, fareyi bırakın. Klavye ok tuşlarına basarak aracı istediğiniz yere götürün.
			** Her iki durumda da aynı anda birden fazla araç hareket ettirilebilir. Bunu fareyle yapmak için Ctrl tuşunu basılı tutun.
			** Araçlar sadece pencere kenarına kadar hareket ettirilebilir.
			
		* Araçların boyutlarını ayarlayabilirsiniz.
			Geometri yöneticisi olarak "place" kullanılmıştır, araç boyutları istendiği gibi değiştirilebilir.
			** Aracı seçin, fare okunu aracın kenarlarına doğru oynatın. Cursor şekil değiştirecektir. Bu pozisyonda "Shift" tuşuna basın ve basılı tutun, aynı zamanda fare sol tuşuna basarak hareket ettirip aracı boyutlandırın.
			** Birden fazla araç seçilerek bunlar aynı anda boyutlandırılabilir, bunun için Ctrl tuşunu basılı tutun.
		
		* Aynı işlemleri, araç çubuğu üzerindeki genişlik, yükseklik, x ve y değerlerini değiştirip Tab tuşuna basarak da yapabilirsiniz.

		* Seçilen araçları üst, alt, sağ veya sol kenarlarına göre hizalayabilirsiniz.
		* Seçilen araçları, en sağ ve en soldaki araçlar arasında eşit aralıkla dağıtabilirsiniz. Aynı şekilde dikey aralıkları da eşitleyebilirsiniz.
		* Seçilen araçları silebilirsiniz.
		* Araçları yeniden adlandırabilirsiniz.
		* Araçların sekme sıralarını ayarlayabilirsiniz. Bunun için aracı seçin, araç çubuğundaki sekme sırası bölümünden bir rakam seçin.
		* Her araç için ipucu metni belirleyebilirsiniz.
		* Font ve renk değiştirmek için fare imlecini özellikler penceresine götürün, ilgili girişe geldiğinizde CTRL+sol tık yapın. Font veya renk değiştirme penceresi açılacaktır. Buradan seçiminizi yapın ve Tamam(OK) düğmesine basarak çıkın. Böyle yapmayıp font veya renk değerlerini elle de girebilirsiniz.
		* Özellikler penceresinde yaptığınız değişikliklerin etkin olması için başka bir yere tıklayın veya Tab tuşuna basın. (bind --> FocusOut)
		* Bir aracı kopyalayabilirsiniz. Aracı seçin, araç çubuğundaki kopyala düğmesine basın. Düğme üzerindeki yazı "yapıştır" olarak değişecektir. Bu durumda bir form üzerine tıklayın ve yapıştır'a tıklayın. Araç, form üzerinde son tıkladığınız yere yapıştırılır. Araç ismini ve isterseniz diğer özelliklerini değiştirin, formu kaydedin.
		*Araç kopyalamak için Ctrl+c tuşlarını kullanabilirsiniz. Yine form üzerinde yapıştıracağınız yere tıklayın ve Ctrl+v tuşlarını kullanarak işlemi tamamlayın.
		* Eğer Shift tuşunu basılı tutarak, fare okunu aracın ortasına getirip sol tık ile süreklerseniz, tuş bırakıldığı anda araç kopyalanacaktır. Bu işlemler, birden fazla aracın seçilmesiyle de yapılabilir.
		* Form üzerine menü oluşturabilir veya daha önce hazırladığınız menüyü düzenleyebilirsiniz.
		* Kayıt sistemini, tabir uygunsa "garantili" yapmaya çalıştım. Değerler önce geçici bir dosyaya yazılıyor, eğer bir hata oluşursa orijinal form dosyası bozulmuyor, yani eskiye dönmek mümkün oluyor. Eğer hata yoksa eski form dosyası siliniyor ve geçici dosyanın adı değiştiriliyor.

	5. Malumunuz, arayüz hazırlamanın amacı, program yazmaktır. Yeni proje oluşturulurken, form dosyası ile birlikte sonu"prg" ile biten bir program dosyası oluşturulur ve içine birşeyler yazılır. Bunları silmeyiniz. Ayrıca button command'lerini özellikler penceresine yazarsanız, bunları kapsayan boş fonksiyonlar program dosyasına kaydedilir. Ancak checkbutton ve radiobutton variable değerlerini program dosyasına yazmalısınız.

	Yapamadıklarım:
	** Yeterli bir modüler yapı oluşturamadım. Programda her öğe birbiriyle bağlantılı, bu yüzden modüller yavaşlamaya ve aksaklığa neden olabiliyor.
	** Dil dosyası yapmayı ve kullanmayı beceremedim, bu yüzden program sadece Türkçe.
	** Kullanıcının ekran çözünürlüğünü tespit ederek pencere boyutlarını ayarlamak isterdim, yapamadım. Bu nedenle sizin bilgisayarınızda pencerelerin boyutları farklı olabilir.
	** Form dosyasını kaydederken Checkbox/Radio button variable değerlerini rakamsal olarak yazdırmayı başaramadım. 








