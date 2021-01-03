# 210103
// CodeUp1473 
  public static void main(String[] args) {
		// TODO Auto-generated method stub
		Scanner sc=new Scanner(System.in);
		int n=sc.nextInt();
		int m=sc.nextInt();
		int[][] arr=new int[n][m];
		int x=1;
		for (int i = n-1; i>=0; i--) {
			if(n%2==0) {
				if(i%2!=0) {
					for (int j = 0; j < m; j++) {
						arr[i][j]=x;
						x+=1;
					}
				}else {
					for (int j = m-1; j >=0; j--) {
						arr[i][j]=x;
						x+=1;
					}
				}
			}
			if(n%2!=0) {
				if(i%2==0) {
					for (int j = 0; j < m; j++) {
						arr[i][j]=x;
						x+=1;
					}
				}else {
					for (int j = m-1; j >=0; j--) {
						arr[i][j]=x;
						x+=1;
					}
				}
			}
			
		}
		
		for (int i = 0; i < n; i++) {
			for (int j = 0; j < m; j++) {
				System.out.print(	arr[i][j]+" ");
			}
			System.out.println();
		}
	}
