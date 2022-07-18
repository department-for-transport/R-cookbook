[![Project Status: WIP – Initial development is in progress, but there has not yet been a stable, usable release suitable for the public.](https://www.repostatus.org/badges/latest/wip.svg)](https://www.repostatus.org/#wip)
  <!-- badges: start -->
  [![CI-CD](https://github.com/department-for-transport/R-cookbook/actions/workflows/CI-CD.yaml/badge.svg)](https://github.com/department-for-transport/R-cookbook/actions/workflows/deploy-bookdown.yaml)
    <!-- badges: end -->
      <!-- badges: start -->
  [![pages-build-deployment](https://github.com/department-for-transport/R-cookbook/actions/workflows/pages-build-deployment.yaml/badge.svg)](https://github.com/department-for-transport/R-cookbook/actions/workflows/pages-build-deployment)
  <!-- badges: end -->

# R-cookbook
https://department-for-transport.github.io/R-cookbook/index.html

## To contribute

If you'd like to make a suggestion on what else should be included, or if you have a better solution to share with us, please raise an issue [here](https://github.com/departmentfortransport/R-cookbook/issues). Alternatively, 

1. Clone or fork the repository
2. Make a new branch for your chapter or changes `git checkout -b name_of_branch`
3. Add/edit content in the `.Rmd` files. 
4. Create a pull request. Please do not include built files in your pull request.
5. An admin will then review the content and either request changes or merge into master (merging into master will trigger the book website to be updated automatically).  

### Using additional packages

If you wish to use a package not already loaded within the book then please add it to the imports section of the `DESCRIPTION` file.

### **lintR**

Please make sure that code sections pass [lintR](https://github.com/jimhester/lintr) checks.  Whilst currently linting errors won't stop the book from building we may in future change this and then any linting errors would cause the build to fail. This would be intentional to ensure the book does not contain any bad practices.

```R
lintr::lint('file.Rmd')
```

