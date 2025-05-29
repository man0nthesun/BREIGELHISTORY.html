<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Питер Брейгель Старший</title>
    <style>
        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
        }
        
        body {
            font-family: 'Times New Roman', serif;
            line-height: 1.7;
            background-color: #f8f5f0;
            color: #333;
            max-width: 1000px;
            margin: 0 auto;
            padding: 20px;
        }
        
        header {
            background: #3a4a5c;
            color: #f0e6d2;
            text-align: center;
            padding: 40px 20px;
            margin-bottom: 30px;
            border-radius: 3px;
            box-shadow: 0 4px 8px rgba(0,0,0,0.1);
            border-bottom: 5px solid #8e7c5e;
        }
        
        h1 {
            font-size: 2.5rem;
            letter-spacing: 1px;
            font-weight: normal;
            text-transform: uppercase;
            font-family: Georgia, serif;
        }
        
        .content {
            background: #ffffff;
            padding: 30px;
            border-radius: 3px;
            box-shadow: 0 2px 12px rgba(0,0,0,0.08);
            border: 1px solid #e0d9c9;
        }
        
        .person-info {
            display: flex;
            flex-direction: column;
            gap: 25px;
            margin-bottom: 30px;
        }
        
        .text-section {
            order: 2;
        }
        
        .image-section {
            order: 1;
            text-align: center;
        }
        
        img {
            max-width: 100%;
            height: auto;
            border-radius: 3px;
            border: 1px solid #d0c9b9;
            box-shadow: 0 3px 6px rgba(0,0,0,0.1);
            margin-bottom: 15px;
            display: block;
        }
        
        .image-caption {
            font-style: italic;
            color: #666;
            font-size: 0.95rem;
            text-align: center;
            margin-top: 5px;
            margin-bottom: 25px;
        }
        
        h2 {
            color: #5a4a32;
            margin-bottom: 20px;
            padding-bottom: 8px;
            border-bottom: 2px solid #e0d9c9;
            font-family: Georgia, serif;
            font-size: 1.8rem;
        }
        
        p {
            margin-bottom: 20px;
            font-size: 1.1rem;
            text-align: justify;
        }
        
        .gallery {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 20px;
            margin: 30px 0;
        }
        
        .gallery-item {
            text-align: center;
        }
        
        .full-width-text {
            width: 100%;
            margin: 40px 0;
            padding: 30px;
            background-color: #f9f7f3;
            border-left: 4px solid #8e7c5e;
        }
        
        .full-width-text h2 {
            color: #3a4a5c;
            border-bottom: none;
            padding-bottom: 0;
        }
        
        /* Стили для новой секции с кликабельной картинкой */
        .clickable-section {
            margin: 50px 0;
            text-align: center;
        }
        
        .clickable-section h2 {
            text-align: center;
            border-bottom: none;
            color: #3a4a5c;
            margin-bottom: 30px;
            position: relative;
            padding-bottom: 15px;
        }
        
        .clickable-section h2:after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 50%;
            transform: translateX(-50%);
            width: 100px;
            height: 3px;
            background: #8e7c5e;
        }
        
        .clickable-image {
            display: inline-block;
            max-width: 90%;
            border-radius: 3px;
            border: 1px solid #d0c9b9;
            box-shadow: 0 5px 15px rgba(0,0,0,0.2);
            transition: all 0.3s ease;
            overflow: hidden;
        }
        
        .clickable-image:hover {
            transform: scale(1.02);
            box-shadow: 0 8px 20px rgba(0,0,0,0.25);
        }
        
        .clickable-image img {
            display: block;
            transition: transform 0.5s ease;
            border: none;
            box-shadow: none;
            margin-bottom: 0;
        }
        
        .clickable-image:hover img {
            transform: scale(1.05);
        }
        
        .image-link-caption {
            display: block;
            margin-top: 15px;
            font-style: italic;
            color: #666;
            font-size: 1rem;
        }
        
        @media (min-width: 768px) {
            .person-info {
                flex-direction: row;
            }
            
            .text-section {
                flex: 3;
                order: 1;
            }
            
            .image-section {
                flex: 2;
                order: 2;
                padding-left: 20px;
            }
            
            .gallery {
                grid-template-columns: repeat(2, 1fr);
            }
            
            .clickable-image {
                max-width: 80%;
            }
        }
        
        @media (max-width: 480px) {
            body {
                padding: 10px;
            }
            
            header {
                padding: 30px 15px;
                margin-bottom: 20px;
            }
            
            h1 {
                font-size: 1.8rem;
            }
            
            h2 {
                font-size: 1.5rem;
            }
            
            .content {
                padding: 20px;
            }
            
            .gallery {
                grid-template-columns: 1fr;
                gap: 15px;
            }
            
            img {
                max-height: 70vh;
            }
            
            .full-width-text {
                padding: 20px;
                margin: 30px 0;
            }
            
            .clickable-section {
                margin: 40px 0;
            }
            
            .clickable-image {
                max-width: 100%;
            }
        }
    </style>
</head>
<body>
    <header>
        <h1>ПИТЕР БРЕЙГЕЛЬ СТАРШИЙ</h1>
    </header>
    
    <main class="content">
        <section class="person-info">
            <div class="text-section">
                <h2>ПИТЕР БРЕЙГЕЛЬ СТАРШИЙ И ЕГО ТЕХНИКА</h2>
                <p>Великий нидерландский живописец Питер Брейгель Старший знаменит своими произведениями живописи. Он является основателем «крестьянского жанра». Брейгель создал многочисленные аллегорические композиции, связанные с народными пословицами и гуманистической культурой своего времени. Блистательный рисовальщик, он также создал ряд подготовительных рисунков для гравирования. Они составляют целый раздел в истории европейского искусства, известный как «Гравюры по Брейгелю».</p>
                <p>В творениях Брейгеля присутствует «мужицкий» юмор в сочетании с трагической иронией. Художник часто говорит притчами, иносказательно, предлагая зрителю поучение и назидание. Он многое оставляет без объяснений и призывает к размышлениям об истинах веры и тайнах Царствия Божьего – земного и небесного.</p>
                <p>Свою творческую деятельность Брейгель начал как гравёр. В начале 1550-х годов художник поселился в Антверпене. Здесь он и начал учиться у преуспевающего живописца и гравёра Питера Кука ван Альста, придворного живописца Карла V. Собственная профессиональная жизнь Брейгеля фактически началась в 1551 году, когда он был избран в Гильдию Святого Луки, антверпенскую ассоциацию художников. Он выполнил множество рисунков для Иеронима Кока, занимавшегося изданием гравюр.</p>
                <p>Огромное влияние на формирование молодого художника оказал его знаменитый соотечественник Иероним Босх, умерший в 1516 году, задолго до рождения Брейгеля. Вероятно, именно в мастерской Кока Брейгель хорошо изучил наследие своего предшественника, копируя его образы и включая мотивы его работ в собственные рисунки. От Босха пошли нелепые и забавные фигурки, вызывающие веселый смех у зрителей. Гравюры, которые Брейгель создавал для своего работодателя, часто содержали юмористические темы и мотивы, за что его и прозвали "Шутник".</p>
                <p>Стиль итальянского ренессанса не оказал на Брейгеля сильного влияния, но сельская местность Италии произвела впечатление на молодого художника, который стал позднее известен своими пейзажными работами. После длительных путешествий во Францию, Италию, Швейцарию Брейгель возвратился на родину и продолжил работать на Иеронима Кока. Он был рисовальщиком в его лавке гравюр, носившей название «На четырех ветрах». По рисункам Брейгеля было выпущено несколько серий гравюр. Среди них – «Большие пейзажи», «Семь смертных грехов», «Семь добродетелей».</p>
                <p>Рисунки Брейгеля, особенно предназначавшиеся для гравировки, обладают четким, прорисованным острым перовым штрихом. В ряде случаев они уже сами имеют вид гравюры.</p>
            </div>
            
            <div class="image-section">
                <img src="https://avatars.mds.yandex.net/get-entity_search/1976572/484897425/S600xU_2x" alt="Портрет Питера Брейгеля Старшего">
                <p class="image-caption">Питер Брейгель Старший</p>
            </div>
        </section>
        
        <section class="gallery">
            <div class="gallery-item">
                <img src="https://artchive.ru/res/media/img/orig/work/b7e/208064.jpg" alt="Альпийский пейзаж">
                <p class="image-caption">Альпийский пейзаж</p>
            </div>
            
            <div class="gallery-item">
                <img src="https://i.pinimg.com/originals/d9/6c/1c/d96c1c2191dd2748163db224a7f8e1c2.png" alt="Падение Икара">
                <p class="image-caption">Падение Икара</p>
            </div>
            
            <div class="gallery-item">
                <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/1/10/Thetriumphofdeath.jpg/960px-Thetriumphofdeath.jpg" alt="Триумф смерти">
                <p class="image-caption">Триумф смерти</p>
            </div>
            
            <div class="gallery-item">
                <img src="https://avatars.mds.yandex.net/i?id=dd9ca28865c2b276ef1a21072457c09ca7600928-5220713-images-thumbs&n=13" alt="Вавилонская башня">
                <p class="image-caption">Вавилонская башня</p>
            </div>
        </section>
        
        <section class="full-width-text">
            <h2>НАСЛЕДИЕ БРЕЙГЕЛЯ В ГРАВЮРЕ</h2>
            <p>Хотя Питер Брейгель Старший наиболее известен своими живописными работами, его вклад в развитие гравюры трудно переоценить. Художник создал более 70 рисунков, специально предназначенных для воспроизведения в гравюре. Эти работы отличаются особой тщательностью проработки деталей и сложной композицией.</p>
            
            <p>Техника Брейгеля в графике уникальна: он использовал перо и чернила, создавая тонкие перекрестные штрихи, которые позволяли передать объем и текстуру. Его рисунки для гравюр характеризуются необычайной детализацией - каждый лист, каждая фигура проработаны с невероятной тщательностью. Особенно впечатляет то, как Брейгель передавал массовые сцены - его композиции содержат десятки, а иногда и сотни персонажей, каждый из которых наделен индивидуальностью.</p>
            
            <p>Гравюры по рисункам Брейгеля оказали огромное влияние на развитие европейского искусства. Они широко распространялись по всей Европе и стали образцом для многих художников. Сегодня эти работы хранятся в крупнейших музеях мира и продолжают восхищать зрителей своей глубиной, юмором и мастерством исполнения.</p>
        </section>
        
        <!-- Новый раздел с заголовком и кликабельной картинкой -->
        <section class="clickable-section">
            <h2>ВИРТУАЛЬНАЯ ВЫСТАВКА ПРОИЗВЕДЕНИЙ</h2>
            <a href="https://docs.google.com/document/d/13sb9dw4r3dD2VAv0S9Gk6SzHZgn1v8HB/edit">
                <img src="https://avatars.mds.yandex.net/i?id=3a4205c8deed22a2979a491c7e63149b_l-4349375-images-thumbs&n=13" alt="Виртуальная выставка работ Брейгеля">
            </a>
            <span class="https://docs.google.com/document/d/13sb9dw4r3dD2VAv0S9Gk6SzHZgn1v8HB/edit">Нажмите на изображение, чтобы узнать информацию о гравюре
        </section>
    </main>
    
    <script>
        // Небольшой скрипт для плавного перехода при клике
        document.querySelectorAll('a[href^="http"]').forEach(anchor => {
            anchor.addEventListener('click', function(e) {
                // Добавляем анимацию перед переходом
                this.style.transform = 'scale(0.95)';
                this.style.opacity = '0.9';
                
                // Небольшая задержка для визуального эффекта
                setTimeout(() => {
                    window.open(this.href, '_blank');
                }, 300);
            });
        });
    </script>
</body>
</html>
