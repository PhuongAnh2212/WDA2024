<template>
  <div>
    <CNavbar expand="lg" color-scheme="dark" class="bg-dark">
      <CContainer fluid>
        <CNavbarBrand href="#">Navbar</CNavbarBrand>
        <CNavbarToggler aria-label="Toggle navigation" :aria-expanded="visible" @click="toggleVisibility"/>
        <CCollapse class="navbar-collapse" :visible="visible">
          <CNavbarNav>
            <CNavItem>
              <CNavLink href="#" active>
                Home
              </CNavLink>
            </CNavItem>
            <CNavItem>
              <CNavLink href="#">Link</CNavLink>
            </CNavItem>
            <CDropdown variant="nav-item" :popper="false">
              <CDropdownToggle color="secondary">Dropdown button</CDropdownToggle>
              <CDropdownMenu>
                <CDropdownItem href="#">Action</CDropdownItem>
                <CDropdownItem href="#">Another action</CDropdownItem>
                <CDropdownDivider />
                <CDropdownItem href="#">Something else here</CDropdownItem>
              </CDropdownMenu>
            </CDropdown>
            <CNavItem>
              <CNavLink href="#" disabled>
                Disabled
              </CNavLink>
            </CNavItem>
          </CNavbarNav>
          <CForm class="d-flex">
            <CFormInput type="search" class="me-2" placeholder="Search"/>
            <CButton type="submit" color="light" variant="outline">Search</CButton>
          </CForm>
        </CCollapse>
      </CContainer>
    </CNavbar>
    <br/>
    <CNavbar expand="lg" color-scheme="dark" class="bg-primary">
      <CContainer fluid>
        <CNavbarBrand href="#">Navbar</CNavbarBrand>
        <CNavbarToggler aria-label="Toggle navigation" :aria-expanded="visible" @click="toggleVisibility"/>
        <CCollapse class="navbar-collapse" :visible="visible">
          <!-- Same navbar content as above -->
        </CCollapse>
      </CContainer>
    </CNavbar>
    <br/>
    <CNavbar expand="lg" color-scheme="light" style="background-color: #e3f2fd">
      <CContainer fluid>
        <CNavbarBrand href="#">Navbar</CNavbarBrand>
        <CNavbarToggler aria-label="Toggle navigation" :aria-expanded="visible" @click="toggleVisibility"/>
        <CCollapse class="navbar-collapse" :visible="visible">
          <!-- Same navbar content as above -->
        </CCollapse>
      </CContainer>
    </CNavbar>
  </div>
</template>

<script>
import {
  CNavbar, CContainer, CNavbarBrand, CNavbarToggler, CCollapse, CNavbarNav, CNavItem, CNavLink, CDropdown, CDropdownToggle, CDropdownMenu, CDropdownItem, CDropdownDivider, CForm, CFormInput, CButton
} from '@coreui/vue'

export default {
  components: {
    CNavbar, CContainer, CNavbarBrand, CNavbarToggler, CCollapse, CNavbarNav, CNavItem, CNavLink, CDropdown, CDropdownToggle, CDropdownMenu, CDropdownItem, CDropdownDivider, CForm, CFormInput, CButton
  },
  data() {
    return {
      visible: false
    }
  },
  methods: {
    toggleVisibility() {
      this.visible = !this.visible
    }
  }
}
</script>

<style>
/* Add any additional styles here */
</style>
