class HelloWorld {
    public static void main(String[] args) {
        String ans="assa";
        int n=ans.length();
        char []ch=ans.toCharArray();
        int s=0; 
        int e=n-1;
        while(s<e){
            char temp=ch[s];
            ch[s]=ch[e];
            ch[e]=temp;
            s++; e--;
        }
        String asha=new String(ch);
        if(asha.equals(ans)){
            System.out.println ("is a palindrome");
        }
        else{
            System.out.println("not a palindrome");
        }
    }
}
