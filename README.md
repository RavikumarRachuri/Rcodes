Rcodes
======
makeCacheMatrix <- function(A=matrix())
{
  # Reading rows and columns
  r <- nrow(A)
  c <- ncol(A)
  if(r==c)
  {
    #calculating the determinant
    d <- det(A)
    if(d==1)
      {
        message("Inverse not possible")
       }
    else{
        matrix <- solve(A)
        return(matrix)
      }    
  }
  message("Inverse wont possible for non-square matrix")
}


cacheSolve <- function(A=matrix())
{
  if(all(solve(A)==A)){
    
    return(A)
  }
  
}
