


public class Dice {
  private static int sRollcount = 0;
  private int nRollcount = 0;

  static int Roll_1_Dice() {
  	sRollcount++;
  	return (int) (1 + Math.random() * 6);
  }

  static int RollDice(int DiceNum, int face) {
  	sRollcount += DiceNum;
  	return (int) (1 + Math.random() * face * DiceNum);
  }

  public static int sRollCount() {

  	return sRollcount;
  }

  public int RollDice() {
  	nRollcount++;
  	return (int) (1 + Math.random() * 6);
  }

  public int RollCount() {

  	return nRollcount;
  }

}
public class Dicemain {
  public static void main(String[] args) {
  	Dice D1 = new Dice();
  	Dice D2 = new Dice();
  	
  	D1.RollDice();
  	D1.RollDice();
  	D2.RollDice();
  	D2.RollDice();
  	D2.RollDice();
  	D2.RollDice();
  	D2.RollDice();
  	System.out.printf("%d\n", D1.RollCount());
  	System.out.printf("%d\n", D1.RollCount());
  	
  	System.out.printf("%d\n ", D2.RollCount() );
  	
  	
  }
}
