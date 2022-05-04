class Power{
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        double num = sc.nextDouble();
        //int pow = (-1)*Integer.MAX_VALUE;
        int pow = sc.nextInt();

        System.out.println(myPow(pow, num));
    }
    public static double myPow(int n, double x) {
        if(n==0 || x == 1){
            return 1;
        }
        if(x == 0){
            return 0;
        }
        if(n == 1){
            return x;
        }
        if(n == -1){
            return 1/x;
        }
        if(x==-1){
            if(n%2==0)
                return 1;
            else
                return -1;
        }

        double product= x;

        int optPow = n;

        if(n%2==0){
            optPow = n/2;
        }else{
            optPow = (Math.abs(n)-1)/2;
        }

        for  (int i=0;i<Math.abs(optPow)-1; i++) {
            product *= x;
        }

        if(n%2==0){
            product *= product;
        }else{
            product *=product * x;
        }

        // Handling for negative powers
        if(n < 0){
            product = 1/product;
        }

        return product;
    }
}
