# Blue-Team---Computer-Networking-Final-Project
Computer Networking

International Computer Networking – Final Project


Projekt obejmował projektowanie, konfigurację i zabezpieczenie infrastruktury sieciowej w środowisku opartym na routerach, switchach i segmentacji VLAN. Celem było odtworzenie rzeczywistych zadań wykonywanych w pracy Network Administrator / Network Engineer / SOC Tier 1, ze szczególnym naciskiem na adresację IP, routing, VLAN-y, OSPF i kontrolę dostępu.

Lab Task 1 – Projektowanie schematu adresacji IP

Pierwszym etapem było zaprojektowanie pełnego planu adresacji dla sieci klasy private 172.16.10.0/24, podzielonej na osiem równych podsieci.

W ramach zadania wykonano:

-obliczenie nowej maski: /27 (255.255.255.224)

-przygotowanie tabeli podsieci z:

-adresami sieci,

-zakresem hostów,

-adresami broadcast,

-analiza liczby dostępnych adresów (30 hostów na podsieć).


Lab Task 2 – Implementacja VLAN i trunking

Zadanie obejmowało konfigurację VLAN-ów oraz trunków na switchach:

-utworzenie VLAN dla różnych segmentów biura (np. Office1, Office2),

-przypisanie interfejsów switcha do odpowiednich VLAN,

-konfiguracja połączeń typu trunk na łączach między przełącznikami (IEEE 802.1Q).

Dzięki temu sieć została logicznie podzielona, co umożliwia separację ruchu i zwiększa bezpieczeństwo.

Lab Task 3 – Przypisanie adresów IP do routerów

W tej części:

-skonfigurowano interfejsy routerów R1, R2 i R3,

-przypisano adresy IP zgodnie ze schematem z Task 1,

-przeprowadzono testy komunikacji między routerami i segmentami VLAN.

To przygotowało środowisko do wdrożenia routingu między VLAN-ami oraz protokołów dynamicznych.

Lab Task 4 – Konfiguracja Inter-VLAN Routing na R1

Router R1 został skonfigurowany jako urządzenie obsługujące routing między VLAN-ami:

-utworzono subinterfejsy (router-on-a-stick),

-przypisano im odpowiednie adresy,

-skonfigurowano enkapsulację dot1Q,

-wykonano testy komunikacji między urządzeniami w różnych VLAN-ach.

Dzięki temu ruch mógł przechodzić między logicznie odseparowanymi sieciami.

Lab Task 5 – Zabezpieczanie portów switchy

W ramach zwiększenia bezpieczeństwa fizycznych portów przełącznika wykonano:

-port security na portach dostępowych,

-ograniczenie liczby MAC adresów,

-blokowanie nieautoryzowanych urządzeń,

-zabezpieczenia przed atakami typu switch spoofing.

To są praktyki stosowane w realnych środowiskach korporacyjnych.

Lab Task 6 – Konfiguracja protokołu OSPF

-W tej fazie projektu wdrożono dynamiczny protokół routingu OSPF na routerach:

-aktywowanie OSPF na interfejsach sieciowych,

-przypisanie router ID,

-konfiguracja sieci w obszarze OSPF,

-weryfikacja tabeli routingu.

Zadanie to jest podstawą nowoczesnych sieci dynamicznie zarządzanych.

Lab Task 7 – Extended ACL

Wykonano konfigurację rozszerzonych list kontroli dostępu (ACL):

-filtrowanie ruchu na podstawie IP źródłowego, docelowego i portów,

-kontrola dostępu do określonych usług,

-zabezpieczenie dostępu między segmentami VLAN.

ACL stanowią kluczowy element bezpieczeństwa sieciowego i są intensywnie wykorzystywane w pracy Network Security.

Lab Task 8 – Ustawienia zabezpieczeń na urządzeniach sieciowych

Na przełącznikach i routerach skonfigurowano podstawowe zabezpieczenia:

-hasła administratora dla konsoli i dostępu uprzywilejowanego,

-szyfrowanie haseł (service password-encryption),

-baner ostrzegawczy (MOTD):

Access to this device is for authorized personnel only!


-zapis konfiguracji (copy running-config startup-config).

To symuluje standardową konfigurację bazową stosowaną przy wdrażaniu nowych urządzeń.

Lab Task 9 – Secure Remote Access

W ostatnim zadaniu wdrożono bezpieczny zdalny dostęp:

-konfiguracja protokołu SSH,

-generowanie kluczy kryptograficznych,

-wyłączenie przestarzałych metod dostępu,

-testy zdalnego logowania.

SSH jest kluczowym narzędziem administracyjnym i elementem bezpieczeństwa operacyjnego.

Efekt końcowy projektu

Projekt pozwolił na praktyczne przećwiczenie:

-projektowania adresacji IP,

-tworzenia VLAN i trunków,

-routingu między VLAN-ami,

-pracy z OSPF,

-zabezpieczania urządzeń sieciowych,

-filtrowania ruchu za pomocą ACL,

-wdrażania bezpiecznego dostępu zdalnego.
