# SO lab 1
public class BaseService {

    public BaseService(double value, String convertTo, String baseCurrency) {
    }

    public double getOutput() {
        // Logica conversiei
        return 0.0; // Rezultatul conversiei (doar un exemplu)
    }
}

public class USDConverter extends BaseService {
    // Variabilele de instanță
    private String baseCurrency = "USD";
    private double value = 0;

    public USDConverter(double _value, String _convertTo) {
        super(_value, _convertTo, "USD");
        value = _value;
    }

    public double convert() {
        return this.getOutput(); // Apelarea metodei din clasa de bază pentru conversie
    }
}
