# DHCP

DORA-Prozess im Detail

    Discover: Der DHCP-Client sendet ein Broadcast-Paket an alle verfügbaren DHCP-Ports bzw. Server. Dies geschieht mit einer Anforderung zur IP-Adressvergabe.

    Offer: Einer oder mehrere Server antworten mit einem Angebot. Dieses enthält eine freie IP-Adresse und andere Konfigurationsparameter.

    Request: Der Client wählt das beste Angebot aus. Er sendet eine Anforderungsnachricht an den jeweiligen Port für DHCP.

    Acknowledge: Der ausgewählte DHCP-Server bestätigt die Zuweisung. Der Client speichert die erhaltenen Konfigurationsdaten lokal.
