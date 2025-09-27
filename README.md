# CGPA-PREDICTOR_
To check the Placement Tier wherein the student lies !

# include <stdio.h>
            void main() {
    float s1,s2,s3,s4,var1,var2,cgpa;
    int c1,c2,c3,c4,skills;
    printf("\t\t\t WELCOME TO THE PLACEMENT PREDICTER\n\n");
    printf("ENTER SGPA(SEMESTER GRADE POINT AVERAGE)FOR THE FIRST SEMESTER\n");
    scanf("%f",&s1);
    printf("ENTER THE CREDITS RECEIVED IN FIRST SEMESTER\n");
    scanf("%d",&c1);
    printf("ENTER SGPA(SEMESTER GRADE POINT AVERAGE)FOR THE SECOND SEMESTER\n");
    scanf("%f",&s2);
    printf("ENTER THE CREDITS RECEIVED IN SECOND SEMESTER\n");
    scanf("%d",&c2);
    printf("ENTER SGPA(SEMESTER GRADE POINT AVERAGE)FOR THE THIRD SEMESTER\n");
    scanf("%f",&s3);
    printf("ENTER THE CREDITS RECEIVED IN THIRD SEMESTER\n");
    scanf("%d",&c3);
    printf("ENTER SGPA(SEMESTER GRADE POINT AVERAGE)FOR THE FOURTH SEMESTER\n");
    scanf("%f",&s4);
    printf("ENTER THE CREDITS RECEIVED IN FOURTH SEMESTER\n");
    scanf("%d",&c4);
     var1=(s1*c1)+(s2*c2)+(s3*c3)+(s4*c4);
     var2= (c1+c2+c3+c4);
     cgpa=var1/var2;
    printf("CGPA OF THE STUDENT is %f", cgpa);
    printf("\nCATEGORISE YOURSELF ON THE BASIS OF THE OPTIONS PROVIDED BELOW \n 1. Strong skills\n 2.Good skills \n 3.Skill development needed \n 4. Needs improvement\n");
    scanf("%d",&skills);
       if(cgpa>9 && skills ==1)
      {
        printf(" TO BE COUNTED IN TIER 1");
      }
      else if(cgpa>8 && cgpa<9 && skills ==2)
      {
           printf("TO BE COUNTED IN TIER 2");
      }
      else if(cgpa>7 && cgpa<8 && skills== 3)
      {
          printf("TO BE COUNTED IN TIER 3");
      }
     else
      {
           printf("TO BE COUNTED IN TIER 4");
      }
    }
