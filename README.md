1. Catching bugs.
2. Typescript compares the object literal against the user.
3. intersection types via & (type B = A & { ... }).
4. we used import and export in Typescript for organization and modularization.
5. Erased, due to the fact JavaScript has no native concept of interfaces.
6. export interface Review {
  id: number;
  userId: number;       
  productId: number;    
  rating: number;      
  comment: string;
  CreatedAt: Date;
}

export interface CreateReviewInput {
  userId: number;
  productId: number;
  rating: number;
  comment: string;
}

export interface UpdateReviewInput {
  rating?: number;      
  comment?: string;     
}
