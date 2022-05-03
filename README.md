# Logtimeline-datalet
Logtimeline-datalet for event-logs visualization in DEEP

Before using this datalet on SPOD, you must add this lines to "\Datalet-Ecosystem-Provider\deep\datalets.xml":

        <!--Logtimeline-->
        <component>
            <name>logtimeline-datalet</name>
            <type>logtimeline</type>
            <idm>
                <inputs>
                    <input>
                        <name>LOGTIMELINEStartDate</name>
                        <description>LOGTIMELINEStartDateDescription</description>
                        <type>TEXT</type>
                        <selection>1</selection>
                    </input>
                    <input>
                        <name>LOGTIMELINEEndDate</name>
                        <description>LOGTIMELINEEndDateDescription</description>
                        <type>TEXT</type>
                        <selection>1</selection>
                    </input>
                    <input>
                        <name>LOGTIMELINEEventTitle</name>
                        <description>LOGTIMELINEEventTitleDescription</description>
                        <type>TEXT</type>
                        <selection>1</selection>
                    </input>
                    <input>
                        <name>LOGTIMELINEEventDescription</name>
                        <description>LOGTIMELINEEventDescriptionDescription</description>
                        <type>TEXT</type>
                        <selection>1</selection>
                    </input>
                    <input>
                        <name>LOGTIMELINEMediaUrl</name>
                        <description>LOGTIMELINEMediaUrlDescription</description>
                        <type>TEXT</type>
                        <selection>?</selection>
                    </input>
                    <input>
                        <name>LOGTIMELINEBackground</name>
                        <description>LOGTIMELINEBackgroundDescription</description>
                        <type>TEXT</type>
                        <selection>?</selection>
                    </input>
                    <input>
                        <name>LOGTIMELINEStartTime</name>
                        <description>LOGTIMELINEStartTimeDescription</description>
                        <type>TEXT</type>
                        <selection>?</selection>
                    </input>
                    <input>
                        <name>LOGTIMELINEFinishTime</name>
                        <description>LOGTIMELINEFinishTimeDescription</description>
                        <type>TEXT</type>
                        <selection>?</selection>
                    </input>
                    <input>
                        <name>LOGTIMELINEEventInfo1</name>
                        <description>LOGTIMELINEEventInfo1Description</description>
                        <type>TEXT</type>
                        <selection>?</selection>
                    </input>
                    <input>
                        <name>LOGTIMELINEEventInfo2</name>
                        <description>LOGTIMELINEEventInfo2Description</description>
                        <type>TEXT</type>
                        <selection>?</selection>
                    </input>
                    <input>
                        <name>LOGTIMELINEEventInfo3</name>
                        <description>LOGTIMELINEEventInfo3Description</description>
                        <type>TEXT</type>
                        <selection>?</selection>
                    </input>
                    <input>
                        <name>LOGTIMELINELink</name>
                        <description>LOGTIMELINELinkDescription</description>
                        <type>TEXT</type>
                        <selection>?</selection>
                    </input>
                    <layouts>
                        <input>
                            <name>date-reading</name>
                            <description>date-readingDescription</description>
                            <type>LIST</type>
                            <selection>1</selection>
                            <list>
                                <item>Std</item>
                                <item>Alt</item>
                            </list>
                        </input>
                        <input>
                            <name>timenav-position</name>
                            <description>timenav-positionDescription</description>
                            <type>LIST</type>
                            <selection>1</selection>
                            <list>
                                <item>Bottom</item>
                                <item>Top</item>
                            </list>
                        </input>
                        <input>
                            <name>lang-timeline</name>
                            <description>lang-timelineDescription</description>
                            <type>LIST</type>
                            <selection>1</selection>
                            <list>
                                <item>en</item>
                                <item>it</item>
                                <item>fr</item>
                                <item>de</item>
                                <item>es</item>
                                <item>cn</item>
                                <item>ja</item>
                            </list>
                        </input>
                        <input>
                            <name>slides-order</name>
                            <description>slides-orderDescription</description>
                            <type>LIST</type>
                            <selection>?</selection>
                            <list>
                                <item>start</item>
                                <item>end</item>
                            </list>
                        </input>
                        <input>
                            <name>LOGTIMELINETheme</name>
                            <description>LOGTIMELINEThemeDescription</description>
                            <type>LIST</type>
                            <selection>?</selection>
                            <list>
                                <item>light</item>
                                <item>dark</item>
                            </list>
                        </input>
                        <input>
                            <name>hash_bookmark</name>
                            <description>hash_bookmarkDescription</description>
                            <type>LIST</type>
                            <selection>?</selection>
                            <list>
                                <item>off</item>
                                <item>on</item>
                            </list>
                        </input>
                    </layouts>
                </inputs>
            </idm>
        </component>

Also, you should add in "\Datalet-Ecosystem-Provider\deep-components\locales\controllet_ln.js" the proper translation for the controllet (english and italian):

ENGLISH:

	//logtimeline english lan
	ln["logtimeline_en"] = "Log timeline";
	ln["logtimelineDescription_en"] = "The logtimeline-datalet is an interactive visualization of event logs on timeline. The event logs are a basic resource that helps provide information about network traffic and other conditions. The events can have a start date and end date or a single date. You also can add the start time and/or end time details from dataset with only time schedule information. You can add event title, event description and other additional event info. It's possible to freely move and zoom the timeline.";
	ln["LOGTIMELINEStartDate_en"] = "Start date";
	ln["LOGTIMELINEStartDateDescription_en"] = "Start date of the event. The logtimeline-datalet supports most of timestamp formats written in log files. For example: the format “yyyy-MM-d’T’HH:mm:ss.SSSZ” (sample value: 2001-07-04T12:08:56.235-0700); the format “yyyyy.MMMMM.dd GGG hh:mm aaa” (sample value: 02001.July.04 AD 12:08:56 -0700); the format “yyyy.MM.dd G ‘at’ HH:mm:ss” (sample value: 2001.07.04 at 12:08:56 PDT).";
	ln["LOGTIMELINEEndDate_en"] = "End date";
	ln["LOGTIMELINEEndDateDescription_en"] = "The end date of the event (see start date). You can use the same information of “Start Date” if the dataset has punctual events.";
	ln["LOGTIMELINEEventTitle_en"] = "Event name";
	ln["LOGTIMELINEEventTitleDescription_en"] = "Event name";
	ln["LOGTIMELINEEventDescription_en"] = "Event description";
	ln["LOGTIMELINEEventDescriptionDescription_en"] = "Event description";
	ln["LOGTIMELINEMediaUrl_en"] = "Media url";
	ln["LOGTIMELINEMediaUrlDescription_en"] = "Url of image or video";
	ln["LOGTIMELINEBackground_en"] = "Background";
	ln["LOGTIMELINEBackgroundDescription_en"] = "URL of background image, CSS colours (for example red, aqua etc.), hexadecimal format (for example # 0f9bd1) or a valid CSS managed colour keyword.";
	ln["LOGTIMELINEStartTime_en"] = "Start Time";
	ln["LOGTIMELINEStartTimeDescription_en"] = "Start time of the event. You can add the time schedule in this input or the full timestamp. The logtimeline-datalet supports these schedule formats: “hh:mm”, “hh:mm:ss”, “hh:mm:ss:ms”, “hh:mm:ss aaa” (for example 12:08:56 -0700), “HH:mm:ssZ” (for example 16:53:34Z), “HH:mm:ss a” (for example 11:31:45 AM) and “hh ‘english time’ a, zzzz” (for example 12 o’clock PM, Pacific Daylight Time).";
	ln["LOGTIMELINEFinishTime_en"] = "Finish Time";
	ln["LOGTIMELINEFinishTimeDescription_en"] = "Finish time of the event. (see start time).";
	ln["LOGTIMELINEEventInfo1_en"] = "Event info 1";
	ln["LOGTIMELINEEventInfo1Description_en"] = "Additional event information.";
	ln["LOGTIMELINEEventInfo2_en"] = "Event info 2";
	ln["LOGTIMELINEEventInfo2Description_en"] = "Additional event information.";
	ln["LOGTIMELINEEventInfo3_en"] = "Event info 3";
	ln["LOGTIMELINEEventInfo3Description_en"] = "Additional event information."
	ln["LOGTIMELINELink_en"] = "Link";
	ln["LOGTIMELINELinkDescription_en"] = "Link";
	ln["date-reading_en"] = "Date reading";
	ln["Std_en"] = "Standard";
	ln["Alt_en"] = "Alternative (first the day)";
	ln["date-readingDescription_en"] = 'The logtimeline read the date in standard mode or in alternative mode (first the day): in standard mode it read the month before the day(for example logtimeline read 10-02-2020 as October, 2); in alternative mode it read the day before the month(for example logtimeline read 10-02-2020 as February, 10).';
	ln["timenav-position_en"] = "Timenav position";
	ln["timenav-positionDescription_en"] = "The position of timeline navigation bar";
	ln["Bottom_en"] = "Bottom";
	ln["Top_en"] = "Top";
	ln["lang-timeline_en"] = "Language";
	ln["lang-timelineDescription_en"] = "The timeline language";
	ln["en_en"] = "English";
	ln["it_en"] = "Italian";
	ln["fr_en"] = "French";
	ln["de_en"] = "German";
	ln["es_en"] = "Spanish";
	ln["cn_en"] = "Chinese";
	ln["ja_en"] = "Japan";
	ln["slides-order_en"] = "Slides loading";
	ln["slides-orderDescription_en"] = 'Load timeline on last or on first slide';
	ln["start_en"] = "On first";
	ln["end_en"] = "On last";
	ln["hash_bookmark_en"] = "Hash bookmark";
	ln["hash_bookmarkDescription_en"] = "If set to ON, logtimeline will update the browser URL each time a slide advances, so that you can link directly to specific slides."
	ln["off_en"] = "OFF";
	ln["on_en"] = "ON";
	ln["LOGTIMELINETheme_en"] = "Theme";
	ln["LOGTIMELINEThemeDescription_en"] = "Theme"
	ln["light_en"] = "Light";
	ln["dark_en"] = "Dark";

ITALIAN:

	//logtimeline italian lan
	ln["logtimeline_it"] = "Log timeline";
	ln["logtimelineDescription_it"] = "La log timeline è una visualizzazione interattiva di event logs su una linea temporale. Gli event logs sono una risorsa di base e forniscono informazioni circa il traffico sulla rete e altre condizioni. Ogni evento ha un timestamp che rappresenta la data in cui si è verificato: nel caso in cui l’evento non è puntuale, ha una data iniziale e una finale. Oltre alla data, è possibile includere le informazioni circa l’orario di inizio e di fine di un evento, il nome, la descrizione, un link e altre informazioni aggiuntive. Inoltre, è possibile spostare e zoomare liberamente la timeline.";
	ln["LOGTIMELINEStartDate_it"] = "DATA INIZIALE";
	ln["LOGTIMELINEStartDateDescription_it"] = "Data iniziale dell'evento. La log timeline supporta la maggior parte dei timestamp scritti nei file di log. Per esempio: il formato “yyyy-MM-d’T’HH:mm:ss.SSSZ” (esempio: 2001-07-04T12:08:56.235-0700); il formato “yyyyy.MMMMM.dd GGG hh:mm aaa” (esempio: 02001.July.04 AD 12:08:56 -0700); il formato “yyyy.MM.dd G ‘at’ HH:mm:ss” (esempio: 2001.07.04 at 12:08:56 PDT). La lista completa dei formati di timestamp supportati è presente a questo link: https://lo901355326.wordpress.com/";
	ln["LOGTIMELINEEndDate_it"] = "DATA FINALE";
	ln["LOGTIMELINEEndDateDescription_it"] = "La data finale dell'evento (vedi data iniziale). Può essere uguale alla data iniziale quando l'evento è puntuale.";
	ln["LOGTIMELINEEventTitle_it"] = "NOME EVENTO";
	ln["LOGTIMELINEEventTitleDescription_it"] = "Nome evento";
	ln["LOGTIMELINEEventDescription_it"] = "DESCRIZIONE EVENTO";
	ln["LOGTIMELINEEventDescriptionDescription_it"] = "Descrizione evento";
	ln["LOGTIMELINEMediaUrl_it"] = "MEDIA URL";
	ln["LOGTIMELINEMediaUrlDescription_it"] = "Url di un'immagine o video";
	ln["LOGTIMELINEBackground_it"] = "IMMAGINE DI SFONDO";
	ln["LOGTIMELINEBackgroundDescription_it"] = "URL di un'immagine di sfondo, colori CSS (ad esempio red, aqua etc.), formati esadecimali (ad esempio # 0f9bd1) oppure una parola chiave valida di un colore gestito con CSS.";
	ln["LOGTIMELINEStartTime_it"] = "ORARIO DI INIZIO";
	ln["LOGTIMELINEStartTimeDescription_it"] = "L'orario di inizio dell'evento. La log timeline supporta questi formati di ora: “hh:mm”, “hh:mm:ss”, “hh:mm:ss:ms”, “hh:mm:ss aaa” (ad esempio 12:08:56 -0700), “HH:mm:ssZ” (ad esempio 16:53:34Z), “HH:mm:ss a” (ad esempio 11:31:45 AM) e “hh ‘english time’ a, zzzz” (ad esempio 12 o’clock PM, Pacific Daylight Time).";
	ln["LOGTIMELINEFinishTime_it"] = "ORARIO DI FINE";
	ln["LOGTIMELINEFinishTimeDescription_it"] = "Orario di fine dell'evento. (vedi orario di inizio).";
	ln["LOGTIMELINEEventInfo1_it"] = "INFORMAZIONE EVENTO 1";
	ln["LOGTIMELINEEventInfo1Description_it"] = "Informazione aggiuntiva dell'evento.";
	ln["LOGTIMELINEEventInfo2_it"] = "INFORMAZIONE EVENTO 2";
	ln["LOGTIMELINEEventInfo2Description_it"] = "Informazione aggiuntiva dell'evento.";
	ln["LOGTIMELINEEventInfo3_it"] = "INFORMAZIONE EVENTO 3";
	ln["LOGTIMELINEEventInfo3Description_it"] = "Informazione aggiuntiva dell'evento."
	ln["LOGTIMELINELink_it"] = "LINK";
	ln["LOGTIMELINELinkDescription_it"] = "Link";
	ln["date-reading_it"] = "Modalità di lettura della data";
	ln["Std_it"] = "Standard";
	ln["Alt_it"] = "Alternativa (prima il giorno)";
	ln["date-readingDescription_it"] = 'La log timeline può leggere la data in modalità standard o alternativa (prima il giorno): in modalità standard legge il mese prima del giorno(ad esempio legge 10-02-2020 come 2 Ottobre); in modalità alternativa legge il giorno prima del mese(ad esempio legge 10-02-2020 come 10 febbraio).';
	ln["timenav-position_it"] = "Posizione del timenav";
	ln["timenav-positionDescription_it"] = "La posizione della barra di navigazione della timeline";
	ln["Bottom_it"] = "Sotto";
	ln["Top_it"] = "Sopra";
	ln["lang-timeline_it"] = "Lingua";
	ln["lang-timelineDescription_it"] = "La lingua della timeline";
	ln["en_it"] = "Inglese";
	ln["it_it"] = "Italiano";
	ln["fr_it"] = "Francese";
	ln["de_it"] = "Tedesco";
	ln["es_it"] = "Spagnolo";
	ln["cn_it"] = "Cinese";
	ln["ja_it"] = "Giapponese";
	ln["slides-order_it"] = "Caricamento diapositive";
	ln["slides-orderDescription_it"] = "Carica la sequenza temporale dalla prima o dall'ultima diapositiva";
	ln["start_it"] = "Dall'inizio";
	ln["end_it"] = "Dalla fine";
	ln["hash_bookmark_it"] = "Segnalibro hash";
	ln["hash_bookmarkDescription_it"] = "Se impostato su ON, la logtimeline aggiornerà l'url del browser per ogni diapositiva, in questo modo è possibile collegarsi direttamente a diapositive specifiche."
	ln["off_it"] = "OFF";
	ln["on_it"] = "ON";
	ln["LOGTIMELINETheme_it"] = "Tema";
	ln["LOGTIMELINEThemeDescription_it"] = "Tema"
	ln["light_it"] = "Chiaro";
	ln["dark_it"] = "Scuro";
	

	
