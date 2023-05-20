# Coding-test
public class OEECalculator {
    public static void main(String[] args) {

double availableTime = 8 * 60;
double breakTime = 1 * 60;
double unplannedDowntime = 2 * 60;
double idealCycleTime = 65;
double noOfOutputs = 5;
double qualityPercentage = 100;

        
double availability = (availableTime - unplannedDowntime) / availableTime;


double performance = (idealCycleTime * noOfOutputs) / (availableTime - breakTime);


double quality = qualityPercentage / 100;


double oee = availability * performance * quality;


System.out.printf("Availability percentage: %.2f%%\n", availability * 100);
        System.out.printf("Performance percentage: %.2f%%\n", performance * 100);
        System.out.printf("Quality percentage: %.2f%%\n", quality * 100);
        System.out.printf("OEE: %.2f%%\n", oee * 100);
    }
}

