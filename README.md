# GPSTrackingDemo
3PT4 Pęczak | GPS &amp; Maps

Niepełne zadanie:
Ile i jakie źródła pozycji możemy wyróżnić w Smartfonach z Androidem?
  GPS - Global Positioning System	
  WI-FI
  wieże telefonii komórkowej
  
Czego potrzebuje aplikacja, by móc odbierać sygnał GPS i wyświetlać użytkownikowi jego pozycję?

Jakie rodzaje dostępu oraz dwa typy lokalizacji oferuje Android?
  Kategoria: lokalizacja na pierwszym planie lub lokalizacja w tle
  Dokładność: dokładna lub przybliżona lokalizacja
  
Jak otrzymywać zmiany pozycji dla Aktywności (Activity)
  uzyskać ostatnio znaną lokalizację
  wykonaj żądanie o lokalizację
  zdefiniuj odpowiedź zwrotną o aktualizacji lokalizacji
  zakończ proces aktualizacji lokalizacji
  
Jak można zamienić koordynaty GPS na adres pocztowy?
  Aby zmienić koordynaty GPS na adres pocztowy możemy użyć usługi Google: Geocode
  np:
  Geocoder geocoder = new Geocoder(this);
        try {
            List<Address> addresses = geocoder.getFromLocation(location.getLatitude(), location.getLongitude(), 1);
            tv_address.setText(addresses.get(0).getAddressLine(0));
        } catch (Exception e) {
            tv_address.setText("Unable to get street address");
        }
