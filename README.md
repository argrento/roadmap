# roadmap
IT Roadmap from https://habrahabr.ru/post/324426/, http://sharpc.livejournal.com/67583.html, 

### Теоретический минимум для программиста
* **C++**
  * стандарт 
  * Comeau
  * 1TBS
  * Страустрап/D&E/Джосаттис/Вандервуд
  * Дьюхэрст/Мейерс/Саттер
  * RAII/copy-and-swap/exception-safety
  * Правило пяти
  * Александреску/Абрахамс-Гуртовой
  * type erasure
  * CRTP
  * NVI
  * SFINAE
  * Koenig lookup
  * Duff's device
  * Boost
  * Сик-Ламсдейн/Карлссон
  * TR on C++ performance 
  * тест Степанова
  * forwarding problem/move semantics
  * SPECS
  * GotW
  * Meyer's singleton
  * cppgm
* **Компиляторы С++**
  * особенности реализации стандарта
  * ограничения реализации
  * интринсики
  * отличия стандартных библиотек (контейнеры, rand)
  * ABI
  * реализация виртуальных функций, виртуального наследования, исключений, RTTI, switch, указателей на функции и методы
  * оптимизации
  * copy elision (RVO, NRVO)
  * sizeof на различных платформах
  * дефайны компилятора и среды
  * __declspec
  * ключи компилятора
  * empty-base optimization
  * статическая и динамическая линковка
  * манглинг
  * распределенная компиляция
  * precompiled header
  * single compilation unit
  * (strict) aliasing/restrict
  * inline/_forceinline
  * volatile
  * быстрое вычисление математических функций через битхаки
  * linkers & loaders by Levine
* **Мультитредность**
  * обедающие философы
  * deadlock/livelock/race condition/starvation
  * атомарность
  * lock инструкции процессора
  * memory model/barrier/ordering
  * CAS или LL/SC
  * wait/lock/obstruction-free
  * ABA problem
  * написание lock-free контейнеров
  * spin-lock
  * TLS/per-thread data
  * закон Амдала
  * OpenMP
  * MPI
  * map-reduce
  * critical section/mutex/semaphore/condition variable
  * WaitForSingleObject/WaitForMultipleObjects
  * green thread/coroutine
  * pthreads
  * future/deferred/promise
  * модель акторов
  * parameter server
  * RDD (as seen in sparks)
  * downpour SGD
  * wait-free
  * stackful vs stackless
* **Язык ассемблера**
  * Зубков/Хайд/Дреппер/Касперски/Фог/Абраш
  * x86
  * FPU/MMX/SSEn/AVX
  * AT&T и Intel-синтаксис
  * masm32
  * макросы
  * стек
  * куча/менеджеры кучи
  * соглашения вызова
  * hex-коды
  * машинное представление данных
  * IEEE754
  * little/big endian
  * SIMD
  * аппаратные исключения
  * прерывания
  * виртуальная память
  * реверсинг
  * срыв стека и кучи
  * return oriented programming
  * alphanumeric shellcode
  * L1/L2/RAM/page fault и их тайминг
  * язык ассемблера ARM
* **Аппаратное обеспечение**
  * Хоровиц-Хилл/Титце-Шенк/От физики к Си от panchul
  * полупроводниковая электроника/спинтроника/фотоника
  * транзистор
  * триггер
  * схемотехника
  * микрокод
  * технология создания процессоров
  * logic synthesis
  * static timing analysis
  * FPGA
  * Verilog/VHDL/SystemC
  * SISAL
  * Arduino
  * устройства памяти (ROM → EEPROM, RAM, SSD, HDD, DVD)
  * RISC/CISC
  * Flynn's taxonomy ([SM]I[SM]D)
  * принстонский и гарвардский подход
  * архитектуры процессоров
  * архитектуры x86
  * VID/PID 
* **Процессоры**
  * конвейеризация
  * hyper-threading
  * алгоритм томасуло
  * спекулятивное исполнение
  * static/dynamic branch prediction
  * префетчинг
  * множественный ассоциативный кэш
  * кэш-линия/кэш-промах
  * такты
  * кольца защиты
  * память в мультипроцессорных системах (SMP/NUMA)
  * тайминг памяти
  * intel optimization manuals
  * performance counters
* **Дискретная математика**
  * K2
  * теорема Поста
  * схемы
  * конечные автоматы (ДКА и НДКА)
  * автомат Калашникова
  * клеточные автоматы
* **Вычислимость**
  * машина Тьюринга
  * нормальные алгоритмы Маркова
  * машина Поста
  * диофантовы уравнения Матиясевича
  * лямбда-функции Черча
  * частично рекурсивные функции Клини
  * комбинаторное программирование Шейнфинкеля
  * Brainfuck
  * эквивалентность тьюринговых трясин
  * проблема останова и самоприменимости
  * счетность множества вычислимых функций
  * RAM-машина
  * алгоритм Тарского
  * SAT/SMT-солверы
  * теория формальных систем
  * interactive proofs
  * теорема Левина-Кука
  * 3SAT
  * PSPACE = NPSPACE
  * #P
* **Языки программирования** 
  * грамматики
  * иерархия Хомского
  * теорема Майхилла-Нероуда
  * лемма о накачке и лемма Огдена
  * алгебра Клини
  * НДКА → ДКА
  * алгоритмически неразрешимые задачи в формальных языках
  * Драгонбук
  * Фридл
  * регекспы и их сложность
  * PCRE
  * БНФ
  * Boost.Spirit + Karma + Qi/Ragel
  * LL
  * LR/SLR/LALR/GLR
  * PEG/packrat
  * yacc/bison/flex/antlr
  * статический анализ кода
  * компиляция/декомпиляция/обфускация/деобфускация
  * Clang/LLVM/XMLVM/Emscripten
  * GCCXML
  * OpenC++
  * построение виртуальных машин
  * JiT/AoT/GC
  * DSL/DSEL
  * on-stack replacement
  * type checking/type inference алгоритмы
  * CYK parser
  * advanced compiler design and implementation by Muchnick
* **Алгоритмы и комбинаторная оптимизация**
  * Кормен/Скиена/Седжвик/Кнут/Ахо-Хопкрофт-Ульман/Пападимитриу/Шрайвер-Голдберг/Препарата-Шеймос/e-maxx.ru
  * структуры данных, алгоритмы, сложность
  * символика Ландау
  * теорема Акра-Баззи
  * time-space tradeoff
  * классы сложности
  * NP-полные задачи
  * КМП
  * графы и деревья
  * потоки в сетях
  * матрица Кирхгофа
  * деревья поиска (особенно RB-дерево и B-дерево)
  * occlusion detection
  * куча
  * хэш-таблицы и идеальный хэш
  * сети Петри
  * алгоритм русского крестьянина
  * метод Карацубы и матричное умножение Винограда-Штрассена
  * сортировки
  * жадные алгоритмы и матроиды
  * динамическое программирование
  * линейное программирование
  * diff-алгоритмы
  * рандомизированные алгоритмы и алгоритмы нечеткого поиска
  * псевдослучайные числа
  * нечеткая логика
  * gusfield (suffix tree, string alignment)
  * motif search
  * scanning line
  * cache oblivious
  * funnel sorting
  * VEB-layout
  * корневая оптимизация
  * алгоритмы для динамических графов 
  * модели вычисления (RAM-machine/pointer machine/decision trees и т.д.)
  * алгоритмы в иерархиях памяти/стриминговые алгоритмы
  * time forward processing
  * range & rank
  * LSM-trees
  * buffered a-b-trees
  * toku trees
  * персистентные структуры
  * succint-структуры
  * lossy-струтуры (bloom/bloomier filter, hash-tables with false positives)
  * locality sensitive hashing
  * space-time tradeoff в хэш-таблицах
  * scheduling strategies
* **Численные методы**
  * дихотомия/метод Ньютона
  * интер- и экстраполяция
  * сплайны
  * метод Гаусса/Якоби/Зейделя
  * QR и LU-декомпозиция
  * SVD
  * МНК
  * методы Рунге-Кутты
  * метод Адамса
  * формулы Ньютона-Котеса
  * метод Ритца
  * метод Бубнова-Галеркина
  * метод конечных разностей/элементов
  * FFT/STFT
  * сходимость и устойчивость
  * l-bfgs и другие квазиньютоновские методы
  * adagrad
  * PARAFAC
  * cassowary
  * interior point methods
  * вариационные методы для байесовского вывода
  * nesterov
  * автоматическое дифференцирование
  * alternating least squares
  * what every computer scientist should know about floating point arithmetics by Goldberg
  * Nocedal & Wright/Boyd & Vandenberghe
* **Машинное обучение**
  * Тибширани/Bishop
  * подходы к моделированию AI
  * переобучение/кроссвалидация
  * байесовские сети
  * нейросети
  * сети Кохонена
  * Restricted Boltzmann machine
  * градиентный спуск/hill climbing
  * стохастическая оптимизация (метод Монте-Карло, метод отжига, генетические алгоритмы, муравьиные алгоритмы)
  * SVM
  * gradient boosting
  * кластерный анализ
  * метод главных компонент
  * LSH
  * обучение с подкреплением
  * MDP
  * information retrieval/data mining/natural language processing
  * машинное зрение
  * Szeliski
  * OpenCV
  * image processing
  * OCR
  * фильтры Собеля
  * каскад Хаара
  * Viola-Jones framework
  * SURF
  * введение в психофизиологию зрения
  * IPython/pandas/scikit-learn
  * (ME)HMM
  * CRF
  * label bias problem
  * stacked NN
  * LeToR
  * factorization machines
  * autoencoders
  * RNN/CNN
  * вместо NLP лучше отдельные задачи (language modelling, co-reference detection, text chunking, POS-tagging, probabilistic parsing, statistical machine translation, misspell correction, question answering, NER, collocation detection, text summarization, speech recognition, fact extraction, sentiment analysis)
  * эффективное вычисление softmax
  * feature engineering/selection
  * quality estimation
  * Manning/Jurafsky/McCallum/Koehn
  * latent topics (LDA, chineese restaurant, pLSI)
  * parallel coordinates
  * vowpal wabbit
  * NLTK
  * structured learning
  * EM-алгоритм
  * contrastive divergence
  * optimal brain surgery
  * belief propagation
  * semi-supervised learning
  * inductive vs transductive learning
  * kernel trick
  * discriminative/generative pairs (as seen by Ng & Jordan)
  * sequence to sequence learning
  * bagging
  * анализ социальных графов
  * рекомендательные системы/collaborative filtering
  * multimodal learning
* **Теория информации**
  * сжатие
  * Хаффман
  * RLE
  * BWT
  * LZ
  * коды коррекции ошибок
  * сжатие с потерями (изображения, аудио, видео)
  * информационная энтропия
  * формула Шеннона
  * сложность Колмогорова
  * maximum entropy problem
  * kullback-leibler divergence
  * elias/shannon-elias encoding
* **Криптография**
  * Шнайер/Ященко
  * Принцип Керкгоффса
  * симметричная (DES, AES)
  * асимметричная (RSA)
  * качество ГПСЧ
  * алгоритм Диффи-Хеллмана
  * эллиптические кривые
  * хэширование (MD5, SHA, CRCn)
  * DHT
  * криптостойкость
  * криптоатаки (атака гроссмейстера)
  * WEP/WPA/WPA2 и атаки на них
  * цифровая подпись и сертификаты
  * PKI
  * HTTPS/SSL
  * доказательство с нулевым разглашением
  * пороговая схема
  * murmurhash/cityhash
  * DKIM
* **Математика**
  * Кнут-Грэхем-Паташник/Зорич/Винберг
  * Spivak/Dummit-Foote
  * матан
  * линал
  * комплан
  * функан
  * диффгем
  * теория чисел
  * дифуры/интуры/урчпы/вариационное исчисление/оптимальное управление
  * производящие функции
  * ряды
  * комбинаторика
  * теорвер/матстат/слупы/теория массового обслуживания
  * цепи Маркова
  * интегральные преобразования (Фурье, Лаплас, вейвлет)
  * NZQRCHOS
  * матпакеты (Mathematica, Maple)
  * теория категорий 
* **Физика**
  * правила Кирхгофа
  * закон Джоуля-Ленца
  * комплексное сопротивление
  * скорость и частота света
  * уравнения Максвелла
  * лагранжиан и гамильтониан
  * quantum tunnelling/hot electron injection :)
* **Химия**
  * стехиометрия
  * химия кремния :)
* **Архитектура и стиль кода**
  * Макконнелл/Фаулер/Лебланк/Гамма/Александреску-Саттер/Буч
  * защитное программирование
  * паттерны
  * SOLID/GRASP/KISS DRY SPOT/YAGNI
  * UML
  * OOP (Smalltalk)
  * OOD/OOA
  * метрики кода
  * uncle Bob
* **Методологии разработки**
  * Waterfall/RUP/Agile/Scrum/Kanban/XP
  * TDD/BDD
  * CASE
* **Тестирование**
  * юнит-тесты
  * функциональное, нагрузочное, интеграционное тестирование
  * тестирование UI
  * mocks/stubs/spies
  * fixture
  * запахи и паттерны тестов (Osherove/Meszaros)
* **Инструментальные средства разработки** 
  * IDE
  * IntelliSense
  * отладчики (VS/Olly/WinDbg/kdb/gdb) и трейсеры (strace/ltrace)
  * DWARF debug information format
  * дизассемблеры и декомпиляторы (IDA/HexRays/Reflector)
  * системы контроля версий (SVN, GIT)
  * merge/branch/trunk
  * системы именования файлов и бранчей
  * continuous integration
  * ant
  * code coverage
  * статический анализ (lint, cppcheck)
  * динамический анализ (valgrind, фаззинг)
  * верификация и валидация ПО (Frama-C, RAISE (RSL), Coq)
  * профайлинг
  * багтрекеры
  * документирование кода
  * системы сборки (CMake)
  * пакетные менеджеры (NuGet)
* **Фреймворки**
  * Qt
  * moc и метаинформация
  * концепция слот-сигнал
  * Саммерфилд-Бланшет/Шлее
  * PoCo
  * промышленные библиотеки: GMP, i18n, lapack, fftw, pcre
* **Операционные системы**
  * Silberschatz/Рихтер/Соломон-Руссинович/Робачевский/Вахалия/Стивенс/Таненбаум/Love/Linux Kernel Internals
  * менеджер памяти
  * менеджер кучи и ее устройство (LAL/LFH/slab)
  * менеджер устройств
  * менеджер процессов
  * context switch
  * реальный и защищенный режим
  * исполнимые файлы (PE/ELF/Mach)
  * объекты ядра
  * отладочные механизмы (strace/ptrace/dtrace/pydbg, Debug API) и минидампы
  * bash
  * сетевой стек и высокопроизводительные сервера
  * netgraph
  * CR0
  * IPC
  * оконная подсистема
  * система безопасности: ACE/ACL и права доступа
  * технологии виртуализации
  * RTOS (QNX)
  * программирование драйверов
  * IRQL
  * IRP
  * файловые системы
  * BigTable
  * NDIS/miniport/FS drivers/filter driver
  * Mm-, Io-, Ldr-функции
  * DKOM и руткиты
  * GDT/IDT/SDT
  * ядра Windows/Linux/BSD
  * POSIX
  * TRIM
* **Компонентно-ориентированные модели**
  * Роджерсон/Таварес
  * COM/OLE/ActiveX/COM+/DCOM RPC
  * ATL
  * апартменты
  * моникеры
  * MIDL
  * XPCOM
  * CORBA
  * TAO
  * D-Bus
* **Сеть**
  * Стивенс
  * OSI model/Internet model
  * Ethernet
  * TCP/IP
  * TCP window
  * алгоритм Нейгла
  * сокеты
  * Protocol buffers/Thrift/Avro/ASN.1
  * AMQP
  * ICMP
  * роутинг/BGP/OSPF
  * ARP
  * атака Митника
  * syn flood
  * HTTP/FTP
  * P2P/DHT
  * DHCP
  * SMB/NBNS
  * IRC/XMPP
  * POP3/SMTP/ESMTP/IMAP
  * DNS
  * WiFi/WiMax/GSM/CDMA/EDGE/Bluetooth/GPS
  * ACE
  * Wireshark
* **Графика и GPGPU**
  * алгоритм Брезенхема
  * цветовые модели
  * трассировка лучей vs полигональная графика
  * OpenGL/GLSL/Open Inventor
  * DirectX/DirectShow/DirectAudio/HLSL
  * stencil/depth/alpha-test
  * графический конвейер в DirectX 11
  * шейдеры
  * модели освещения (Фонг)
  * пропускная способность
  * fillrate
  * OpenCL/CUDA/AMP
  * ландшафты
  * лоды
  * тени
  * deferred shading
  * текстурирование и фильтрация
  * антиалиасинг
  * HDR
  * tone mapping
  * virtual/augmented reality  
* **Форматы**
  * XML/XSLT/XPath/XMLStarlet/DOM/SAX
  * RTF/ODF
  * JSON/BSON/bencode
  * YAML
  * JPEG/PNG/WebP
  * AVI/MPEG/RIFF/WAV/MP3/OGG/WebM
  * SVG
  * Unicode
  * кодировки однобайтные/UTF-8/UTF-16/UCS-2/UTF-32
  * проблемы длины и сравнения Unicode-строк
  * base64
  * markdown
* **Базы данных/Распределенные системы**
  * Грубер/Дейт
  * ANSI SQL
  * T-SQL
  * ODBC
  * MySQL/PostgreSQL/MS SQL/BDB/SQLite/Sphinx
  * хранимые процедуры
  * триггеры
  * алгебра Кодда/А
  * Tutorial D
  * нормальные формы
  * оптимизация и выполнение запросов
  * структуры данных индексов
  * транзакции и ACID
  * CAP-теорема Брюера
  * graph DB
  * document store
  * wide column store
  * key-value storage
  * теория распределенных систем
  * CRDT
  * net split проблема
  * протоколы консенсуса
  * теория шардинга/репликации
  * ORM (C++ ODB)
  * ERD
  * OLAP
  * семантическая сеть
  * triplestore
  * RDF/Turtle
  * SPARQL
  * OWL
  * Semanticscience Integrated Ontology
  * reasoner
  * DBpedia
  * big table/hbase vs. dynamodb/cassandra/riak
  * 2/3PC
  * chubby/zoo keeper
  * leader election (paxos/raft)
  * hdfs/gfs/glusterfs
  * deduplication problem
  * causality detection (vector clock/stamps)
  * R/W quorum
  * load balancing
  * устройство индексов поисковых систем
  * event sourcing
  * CRDT
  * дизайн протоколов и принципы коммуникации с точки зрения эволюции, расширяемости, надежности
  * дизайн программных интерфейсов (API)
* **Прикладное программирование**
  * C#/F#
  * Шилдт/Троелсен/Рихтер
  * генерики
  * yield
  * linq/plinq
  * рефлексия
  * AST
  * WCF
  * WinForms/WPF/Silverlight
  * AOP
  * фреймворки логгирования
  * .NET assembly
  * Scala
  * Хорстманн/Одерски
  * pattern matching
  * макросы/квазицитаты
* **Квантовые вычисления**
  * алгоритм Шора
  * квантовая криптография
* **Функциональное программирование**
  * Haskell/Ocaml/Scheme/Alice или Oz
  * SICP/TaPL/YAHT/Purely Functional Data Structures/Харрисон-Филд
  * HOF (map/fold/filter)
  * система типов Хиндли-Милнера
  * монады
  * тайпклассы
  * АТД
  * dependent types
  * ленивость/энергичность
  * логическое программирование (Prolog или Mercury)
  * конкурентное программирование (Erlang или Oz)
* **Веб-программирование и скриптовые языки**
  * Фланаган/Zend PHP5 Certification Course + Study Guide
  * Apache/nginx
  * CGI/FastCGI
  * PHP/Zend Framework/ReactPHP/Zend Engine/Doctrine или Propel/CodeIgniter или Symphony или Yii
  * Python/Django/Twisted
  * Ruby/RoR
  * ASP.NET MV*
  * JavaScript/jQuery/React/Google Closure/ExtJS/node.js
  * ООП в JavaScript
  * HTML5
  * CSS3/табличная и блочная верстка
  * RSS
  * canvas/WebGL
  * Ajax/WebSockets
  * вопросы безопасности (XSS, SQL injection, CSRF)
  * highload
  * C10k problem
  * SWIG
  * CDN
  * shadow DOM
  * квирки браузеров
  * real time bidding/trading
  * anomaly detection
  * архитектура single page apps
  * устройство веб-краулеров
  * web/social graph random walk
  * asm.js и компиляция в js
  * v8/spidermonkey internals
  * PaaS/IaaS
  * SPDY
* **Проектирование GUI и представление информации**
  * Раскин/Тафти
  * юзабилити
  * основы дизайна и типографики
  * закон Фиттса
  * основы верстки
  * LaTeX
  * алгоритмы визуализации данных (as seen in d3)
  * subpixel rendering  
